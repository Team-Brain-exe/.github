# Trauma Route System

### Connected Emergency-Response Platform

The Trauma Route project is a multi-component emergency-response platform consisting of a central backend server and two dedicated frontend applications for hospitals and paramedics.

The three repositories work together as one system. The server provides shared API, database and real-time communication infrastructure for both clients.

## System Architecture

```text
                 trauma-route-server
              Node.js + Express.js
                 MongoDB + Mongoose
                     Socket.IO
                         |
                REST API + WebSockets
                         |
            +------------+------------+
            |                         |
   trauma-route-hospital     trauma-route-paramedic
      React + Vite                React + Vite
   Hospital-facing UI          Paramedic-facing UI
```

## Components

### 1. Trauma Route Server

The central backend component. It handles API requests, database operations and real-time communication between connected clients.

**Technology stack:** Node.js, Express.js, MongoDB, Mongoose, Socket.IO, CORS, dotenv, Nodemon, Docker.

Repository: [trauma-route-server](https://github.com/Team-Brain-exe/trauma-route-server)

### 2. Trauma Route Hospital

The hospital-facing frontend application. It communicates with the central server through REST APIs and real-time Socket.IO connections.

**Technology stack:** React 19, Vite, React Router DOM, Axios, Socket.IO Client, ESLint, Nginx, Docker.

Repository: [trauma-route-hospital](https://github.com/Team-Brain-exe/trauma-route-hospital)

### 3. Trauma Route Paramedic

The paramedic-facing frontend application. It communicates with the central server using REST APIs and real-time Socket.IO connections.

**Technology stack:** React 19, Vite, React Router DOM, Axios, Socket.IO Client, ESLint, Nginx, Docker.

Repository: [trauma-route-paramedic](https://github.com/Team-Brain-exe/trauma-route-paramedic)

## Combined Technology Stack

| Layer | Technologies |
|---|---|
| Frontend clients | React 19, Vite, React Router DOM, Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Real-time communication | Socket.IO |
| Configuration / Development | dotenv, Nodemon, ESLint |
| Deployment | Nginx, Docker |

## Repositories

- [Server](https://github.com/Team-Brain-exe/trauma-route-server)
- [Hospital](https://github.com/Team-Brain-exe/trauma-route-hospital)
- [Paramedic](https://github.com/Team-Brain-exe/trauma-route-paramedic)
