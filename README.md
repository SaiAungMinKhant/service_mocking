# Service Mocking Project

This project demonstrates a service mocking setup with a static web application and a mock API server. It showcases how to create a frontend application that consumes data from a mock backend service.

## Project Structure

```
service_mocking/
├── static/                 # Static web application
│   ├── app.js             # Frontend application logic
│   └── index.html         # Main HTML file
├── mock-srv/              # Mock API server
│   ├── routes/            # API routes
│   │   ├── electronics/   # Electronics products API
│   │   └── confectionery/ # Confectionery products API
│   └── app.js            # Main server application
├── server_example.mjs     # Example server implementation
└── package.json          # Project dependencies and scripts
```

## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## Setup

1. Install dependencies for the main project:
```bash
npm install
```

2. Install dependencies for the mock server:
```bash
cd mock-srv
npm install
cd ..
```

## Running the Application

### 1. Start the Mock API Server

In one terminal:
```bash
cd mock-srv
npm run dev
```

The mock server will start on http://localhost:3000

### 2. Start the Static Web Server

In another terminal:
```bash
npm run static
```

The static web application will be served on http://localhost:5050

## Features

- Static web application with product listing
- Mock API server with two endpoints:
  - `/electronics` - Returns electronics products
  - `/confectionery` - Returns confectionery products
- Example server implementation for reference

## API Endpoints

### Electronics Products
- URL: `http://localhost:3000/electronics`
- Method: GET
- Response: JSON array of electronics products

### Confectionery Products
- URL: `http://localhost:3000/confectionery`
- Method: GET
- Response: JSON array of confectionery products

## Development

- The static web application is built using vanilla JavaScript and Web Components
- The mock server is built using Fastify
- The example server demonstrates a simple Node.js HTTP server implementation

## Author

Sai Aung Min Khant

## License

ISC