# RideXpress

## 🚀 Project Overview

**RideXpress** is a ride-hailing application backend that facilitates seamless ride booking, management, and real-time communication between users and drivers (captains). It supports user registration, ride creation and tracking, driver management, and real-time updates using WebSockets.

---

## ✨ Features

- User and Driver (Captain) registration and authentication
- Ride creation, update, and status management
- Real-time ride updates via WebSockets
- Map-related services (likely route or location fetching)
- Secure route handling with authentication middleware

---

## 🛠 Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB (via Mongoose ODM)
- **Authentication**: JWT-based authentication with token blacklisting
- **Real-time Communication**: WebSockets (via `socket.io`)
- **Other Tools**: `dotenv`, `cors`, `bcrypt`, `morgan`, etc.

---

## 📁 Folder Structure

```
RideXpress-main/
│
├── Backend/
│   ├── controllers/          # Handles the business logic for each route
│   ├── db/                   # Database connection configuration
│   ├── middlewares/          # Middleware for authentication and others
│   ├── models/               # Mongoose models for MongoDB collections
│   ├── routes/               # Express route definitions
│   ├── app.js                # Main app initialization
│   ├── server.js             # Starts the server
│   ├── socket.js             # Socket.IO setup for real-time communication
│   └── package.json          # Project metadata and dependencies
│
└── README.md                 # Project description and usage
```

---

## 📌 Additional Notes

- **Authentication Middleware**: The app uses token-based auth with token blacklisting for logout functionality.
- **WebSocket Integration**: Real-time features (e.g., ride updates) are powered by `socket.io` in `socket.js`.
- **Modular Structure**: Code is well-structured in MVC format separating routes, controllers, and models.

---
