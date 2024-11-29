# VRV Security System

This project is a security management system built with a client-server architecture. The system allows users to register, log in, and access various services based on their role (e.g., Guard, Manager, Authority). It uses Node.js, Express, MongoDB for the backend, and React for the frontend.

## Features

- **User Authentication**: Users can sign up, log in, and authenticate using JWT.
- **Role-based Access**: Different services are available based on user roles (e.g., Guard, Manager, Authority).
- **Services**:
  - CCTV Surveillance
  - Guard Deployment Management
  - Attendance Records
  - Active Units Management

## Tech Stack

### Backend:
- **Node.js**: JavaScript runtime to run the server.
- **Express.js**: Web framework for Node.js to handle routing and requests.
- **MongoDB**: NoSQL database for storing user data and application-related information.
- **JWT**: JSON Web Token for secure user authentication.

### Frontend:
- **React.js**: A JavaScript library for building user interfaces.
- **CSS/TailwindCSS**: Styling and layout for the UI components.

## Installation

### 1. Clone the repository

Run the following command to clone the repository:

git clone https://github.com/Sparsh190/Vrv-security.git

cd vrv-assignment-master
2. Install dependencies for backend and frontend

Backend:

Navigate to the server directory and install the required dependencies:
cd server
npm install
Frontend:

Navigate to the client directory and install the required dependencies:
cd client
npm install
Set up environment variables

Create a .env file in the server directory and add the following:
CONNECTION_URL=<Your_MongoDB_Connection_URL>
SECRET_KEY=<Your_Secret_Key>
Replace <Your_MongoDB_Connection_URL> with your MongoDB connection string.
	•	Replace <Your_Secret_Key> with a secret key for JWT token generation.
 
 4. Start the server and client

Backend:

After installing dependencies, start the backend server:
cd server
npm start
Frontend:

Once the backend is running, navigate to the client directory and start the frontend:
cd client
npm start
Now, the backend should be running on http://localhost:5000 (or your chosen port) and the frontend should be available at http://localhost:3000.

Usage

	1.	Sign Up / Log In:
	•	Go to the frontend and register as a user by providing the employee_id, role, phone, and password.
	•	Log in with the employee_id and password to get an authentication token.
	2.	Access Services:
	•	Based on your role, you will have access to different services such as CCTV surveillance, guard deployment management, attendance records, and active unit management.
 vrv-assignment-master/
│
├── client/              # React frontend
│   └── src/             # React components and views
│
├── server/              # Node.js/Express backend
│   └── models/          # MongoDB models
│   └── routes/          # API routes for authentication and services
│   └── controllers/     # Business logic
│   └── .env             # Environment variables for backend
│
├── package-lock.json    # Lock file for Node.js packages
└── README.md            # This file
