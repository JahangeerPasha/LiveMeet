# LiveMeet – Real-Time Video Conferencing Platform

LiveMeet is a real-time video conferencing application built using **WebRTC**, **Socket.io**, **Node.js**, and **Express.js**.  
It enables seamless peer-to-peer video/audio calls, dynamic room creation, and real-time communication with extremely low latency.

---

## 🚀 Features

### 🔹 Real-Time Video & Audio Calls
- Powered by **WebRTC** for direct peer-to-peer media streaming.
- Handles live audio/video sharing with smooth connection handling.

### 🔹 STUN Server Support  
- Integrated **Google STUN servers** to enable reliable **NAT traversal**.
- Ensures stable connectivity across different networks.

### 🔹 Socket.io Signaling
- Real-time room creation and joining.
- WebSocket-based event communication:
  - User joined
  - Call requests
  - Media updates
  - Disconnections  

### 🔹 Dynamic Peer Connection Management
- Automatically handles:
  - New peers joining
  - Peers leaving
  - ICE candidate exchange
  - Stream updates

### 🔹 Responsive UI
- Clean and simple UI for easy room joining and interaction.
- Mobile-friendly layout supporting both portrait/landscape usage.

---

## 🛠️ Tech Stack

### **Frontend**
- HTML5, CSS3, JavaScript
- WebRTC API (getUserMedia, RTCPeerConnection)
- Responsive UI design

### **Backend**
- Node.js  
- Express.js  
- Socket.io (WebSocket communication)

### **Real-Time Communication**
- WebRTC for video/audio  
- STUN servers for NAT traversal  
- Peer-to-peer streaming  

### **Tools & Concepts**
- ICE Candidates  
- SDP Exchange  
- WebSocket Rooms  
- Event-driven architecture  

---

## 🧩 How It Works (Architecture)

1. User enters a room ID.
2. Socket.io connects them to a signaling room.
3. WebRTC performs:
   - Offer/Answer exchange
   - ICE candidate communication
4. Peers establish a **direct P2P connection**.
5. Video/audio streams flow **directly** between devices.


