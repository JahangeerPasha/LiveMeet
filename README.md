# LiveMeet – Real-Time Video Conferencing Application

LiveMeet is a web-based real-time video conferencing application that allows users to securely create and join meetings using a unique meeting code. The platform supports live audio/video communication, screen sharing, real-time chat, and meeting history tracking. It demonstrates how modern video conferencing systems are built using WebRTC with a hybrid client-server and peer-to-peer architecture.

## 🌐 Live Demo

🔗 **Deployed Link:**  
https://livemeet-frontend.onrender.com

> Note: The application may take a few seconds to load initially as it is deployed on a free hosting service.

---

## 🚀 Features

- User Authentication (Register & Login)
- Create and Join Meetings using Meeting Code
- Real-Time Video and Audio Calling
- Screen Sharing
- Camera and Microphone Toggle
- Real-Time Chat during Meetings
- Meeting History Tracking
- Protected Routes for Authenticated Users

---

## 🛠 Tech Stack

### Frontend
- React
- React Context API
- Material UI
- CSS Modules
- Socket.IO Client
- WebRTC Browser APIs

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- Socket.IO
- bcrypt
- crypto

---

## 🏗 Architecture Overview

LiveMeet follows a **hybrid architecture**:

- **Client–Server Architecture** for authentication, authorization, and meeting history
- **Peer-to-Peer Architecture** for real-time audio and video streaming using WebRTC

The backend manages users and signaling, while media streams flow directly between browsers, ensuring low latency and reduced server load.

---

## 🔁 How the System Works

1. User registers or logs in to the application.
2. Backend validates credentials and returns an authentication token.
3. Authenticated users create or join a meeting using a meeting code.
4. Socket.IO handles real-time signaling and chat communication.
5. WebRTC establishes peer-to-peer connections between participants.
6. Audio and video streams flow directly between browsers.
7. Meeting history is stored in MongoDB and can be accessed later.

---

## 🔐 Authentication & Security

- Passwords are hashed using **bcrypt** before storing in the database.
- Token-based authentication is used to keep the backend stateless.
- Frontend route protection prevents unauthorized access.

---

## 🌐 Real-Time Communication

- **Socket.IO** is used for signaling (user join/leave, SDP, ICE exchange).
- **WebRTC** handles peer-to-peer audio and video streaming.
- **STUN servers** are used for NAT traversal.
