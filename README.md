ChatBot WebSockets
A real-time chat application using WebSockets for instant messaging capabilities.
Overview
This project implements a full-featured chat application using WebSocket technology to provide real-time communication. The system supports both one-on-one conversations and group chats with instant message delivery and status updates.
Features

Real-time Communication: Instant message delivery using WebSockets
User Authentication: Secure login and registration system
One-on-One Chat: Private conversations between users
Group Chat: Multiple users can join conversation rooms
Message History: Persistent storage of chat messages
Online Status: Real-time user presence indicators
Typing Indicators: Shows when users are typing
Read Receipts: Confirmation when messages are seen
Responsive Design: Works across devices and screen sizes

Tech Stack

Frontend:

HTML5, CSS3, JavaScript
React.js for UI components
Socket.io client for WebSocket connections


Backend:

Node.js runtime environment
Express.js framework
Socket.io for WebSocket implementation
MongoDB for message and user data storage
JWT for authentication



Architecture
The application follows a client-server architecture:

Client Application: React-based frontend that maintains a WebSocket connection
WebSocket Server: Handles real-time message routing and broadcasting
REST API: For authentication and data retrieval
Database: Stores user profiles, conversation history, and message data

Getting Started
Prerequisites

Node.js (v14 or higher)
MongoDB
npm or yarn

Installation

Clone the repository:
bashCopygit clone https://github.com/pisatishivatmika/ChatBot-websockets.git
cd ChatBot-websockets

Install backend dependencies:
bashCopycd server
npm install

Install frontend dependencies:
bashCopycd ../client
npm install

Create a .env file in the server directory with the following variables:
CopyPORT=5000
MONGODB_URI=mongodb://localhost:27017/chatbot
JWT_SECRET=your_jwt_secret_key


Running the Application

Start MongoDB:
bashCopymongod

Start the backend server:
bashCopycd server
npm start

Start the frontend development server:
bashCopycd client
npm start

Access the application at http://localhost:3000
