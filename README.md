# Authentication App

A modern, full-stack authentication platform designed to provide secure user registration and login functionality with a beautiful, responsive interface.

## Problem Statement

Users need a simple and secure way to create accounts and authenticate themselves in web applications. This system provides a unified authentication solution with password visibility controls and seamless navigation between login and signup pages.

## System Architecture

**Architecture Overview:**

Frontend (ReactJS + Tailwind CSS)
↓
Backend (Node.js + Express)
↓
Database (MongoDB)

**Flow Description:**

- **Frontend:**
  Built using ReactJS with React Router for navigation and Tailwind CSS for modern, responsive design. Includes password visibility toggles and form validation.

- **Backend:**
  RESTful API using Node.js and Express, managing authentication, user registration, and secure password handling.

- **Database:**
  MongoDB stores user data with encrypted passwords and user information.

- **Authentication:**
  JWT-based authentication for secure sessions, and bcrypt for password encryption.

## Key Features

| Category | Features |
|----------|----------|
| **User Registration** | Sign up with full name, email, password, and confirm password fields |
| **User Login** | Secure login with email and password authentication |
| **Password Security** | Password visibility toggle buttons, bcrypt hashing, minimum length validation |
| **UI & Design** | Beautiful gradient backgrounds, responsive Tailwind CSS design, smooth transitions |
| **Navigation** | Seamless navigation between login and signup pages |
| **State Management** | React state management for form inputs and error handling |
| **Real-Time Validation** | Client-side and server-side validation with error messages |

## Tech Stack

| Layer | Technologies Used |
|-------|------------------|
| Frontend | React.js, React Router, Tailwind CSS, Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| Authentication | JWT, bcrypt |

## Setup

### Backend

1. Navigate to the backend folder and install dependencies:
```bash
cd backend
npm install
```

2. Create a `.env` file in the backend folder with:
```
MONGODB_URI=mongodb+srv://aloktomar2024_db_user:K1sp3cXMtUTSyDSZ@cluster0.jpzja0x.mongodb.net/?appName=Cluster0
JWT_SECRET=aed31aa5a7bf5b00a4350ba397b843d3b7aa7a7d6a7abd494942a79f1eafe017af22d65878278243dd3798334e2ab0fec3010d4b7a94ba80bd756d2bcfeb5427
PORT=5001
```

3. Start the server:
```bash
npm start
```

### Frontend

1. Navigate to the frontend folder and install dependencies:
```bash
cd frontend
npm install
```

2. Create a `.env` file in the frontend folder with:
```
REACT_APP_API_URL=http://localhost:5001
```

3. Start the development server:
```bash
npm start
```

The app will open at `http://localhost:3000`

## Expected Outcome

- A fully functional authentication system with modern UI and secure backend logic.
- Enhanced user experience through password visibility controls and intuitive navigation.
- Demonstration of full-stack proficiency in REST API design, frontend state management, and secure authentication practices.

