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

## ⚙️ Installation & Setup

```bash
# Navigate to Backend directory
cd Backend

# Install dependencies
npm install

# Set up your environment variables in a `.env` file
touch .env
# Add the required variables like:
# PORT=5000
# MONGODB_URI=your_mongo_uri
# JWT_SECRET=your_jwt_secret

# Run the server
npm start
```

---

## ▶️ How to Run

To start the backend server:

```bash
node server.js
```

Make sure MongoDB is running locally or that you have a remote MongoDB connection string in your `.env` file.

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
