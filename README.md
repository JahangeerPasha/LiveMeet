# LiveMeet
LiveMeet is a real-time video conferencing platform built using WebRTC, Socket.io, and Node.js.
The platform enables peer-to-peer audio/video communication, dynamic room creation, and real-time signaling, while ensuring reliable connectivity using STUN servers for NAT traversal.

This project demonstrates expertise in real-time communication, networking concepts, WebRTC internals, and scalable event-driven backend systems.

This project demonstrates strong understanding of:

Real-time communication systems

Signaling mechanisms

Peer connection lifecycle

Scalable event-driven backend architecture

 Features

✔ Peer-to-peer video calling using WebRTC
✔ STUN-based NAT traversal for stable connectivity
✔ Room-based video calls (auto-generate & join)
✔ Real-time signaling using Socket.io
✔ Dynamic peer connection management
✔ Responsive UI for smooth user experience
✔ Low-latency media streaming
✔ Automatic handling of new participants and disconnections

 Architecture

LiveMeet follows a hybrid architecture:

1️⃣ WebRTC (Media Layer)

Handles audio/video capture

Establishes direct P2P connections

Uses ICE candidates for connection optimization

2️⃣ Socket.io (Signaling Layer)

Used ONLY for exchanging connection metadata:

Offer / Answer (SDP)

ICE candidates

Join/leave notifications

Event-driven communication between clients

3️⃣ Node.js + Express.js (Backend Server)

Hosts signaling server

Manages room logic

Handles event broadcasting

Lightweight real-time message handling

🛰️ Tech Stack
Frontend

HTML

CSS

JavaScript

WebRTC API

MediaDevices API

Backend

Node.js

Express.js

Socket.io

Networking

STUN (Google STUN Server)

ICE Framework

Peer Connection API

How It Works
1️⃣ User creates or joins a room

Client sends a join-room event to the server.

2️⃣ Server broadcasts signaling events

Notifies existing users

Exchanges SDP offers/answers

Shares ICE candidates

3️⃣ WebRTC establishes a P2P connection

Browser-to-browser communication begins:

No heavy backend load

Low latency

4️⃣ Video + Audio stream starts

Media is streamed directly through P2P once ICE negotiation succeeds.

 Key Concepts Implemented
✔ WebRTC PeerConnection Lifecycle

Offer → Answer → ICE Exchange → Connected

✔ STUN Server Integration

Ensures:

NAT traversal

Accurate public IP discovery

Stable connectivity across networks

✔ Real-Time Signaling with Socket.io

Handles:

User joining

Broadcasting offers/answers

ICE candidate exchange

✔ Dynamic Stream Handling

Automatically attach new video streams

Remove streams when a user disconnects
