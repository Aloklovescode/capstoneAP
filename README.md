# Production – Smart Kanban Project Management App

A modern, full-stack project management platform designed to help teams organize tasks, collaborate efficiently, and visualize workflows using draggable Kanban boards — now enhanced with advanced search, sorting, filtering, and pagination functionalities.

## Problem Statement

In most project management tools, users face difficulty managing large numbers of projects, tasks, and notes across various platforms — leading to confusion, inefficiency, and decreased productivity.

Productio aims to provide a unified, intelligent Kanban-style project management system where users can easily create, organize, and track projects in one place.

The system now includes:
- Advanced Search and Filtering to quickly locate tasks and boards.
- Sorting and Pagination to manage large datasets efficiently.
- Interactive drag-and-drop Kanban interface for seamless organization.

This ensures faster information retrieval, better productivity, and a more professional user experience.

## System Architecture

**Architecture Overview:**

Frontend (ReactJS + Material UI)
↓
Backend (Node.js + Express)
↓
Database (MongoDB)

**Flow Description:**

- **Frontend:**
  Built using ReactJS with Redux for state management, React Beautiful DnD for drag-and-drop, and Material UI for an interactive, responsive design. Includes search bars, filters, and pagination UI for boards and tasks.

- **Backend:**
  RESTful API using Node.js and Express, managing authentication, CRUD operations, and data retrieval with query-based search, sorting, and pagination logic.

- **Database:**
  MongoDB Atlas stores user data, boards, sections, and tasks with indexing for optimized search and sort operations.

- **Authentication:**
  JWT-based authentication for secure sessions, and bcrypt for password encryption.

- **Hosting:**
  - Frontend → Vercel
  - Backend → Render
  - Database → MongoDB Atlas

## System Architecture Diagram (Text Representation)

[React Frontend] → [Express REST API] → [MongoDB Atlas]
↑ ↓
JWT Auth CRUD + Search/Sort Logic
↑ ↓
Redux State Optimized Querying + Pagination

## Key Features

| Category | Features |
|----------|----------|
| **Authentication & Security** | Secure signup/login with JWT and bcrypt password hashing. |
| **Boards Management** | Create, edit, and delete boards; drag-and-drop sections and tasks using React Beautiful DnD. |
| **Sections & Tasks** | Add sections to boards and create tasks; each task has notes and due dates. |
| **Search, Sort, Filter, Pagination** | Search boards or tasks by title or tag, filter by status or priority, sort by date or name, and paginate results for performance. |
| **Favorites** | Mark boards as favorites for quick access. |
| **UI & Personalization** | Toggle between dark/light modes; responsive Material-UI design. |
| **State Management** | Efficient state control with Redux for real-time updates. |
| **Real-Time Data** | All user actions are synced instantly through MongoDB. |
| **Hosting & Deployment** | Frontend on Vercel, Backend on Render, Database on MongoDB Atlas. |

## Tech Stack

| Layer | Technologies Used |
|-------|------------------|
| Frontend | React.js, Redux, Material-UI, React Beautiful DnD |
| Backend | Node.js, Express.js |
| Database | MongoDB (Indexed for search/sort/pagination) |
| Authentication | JWT, bcrypt |
| Search/Filter Logic | MongoDB queries + Express API parameters |
| Hosting | Vercel (Frontend), Render (Backend), MongoDB Atlas (Database) |

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

- A fully functional Kanban-style project management app with modern UI and backend logic.
- Enhanced usability through search, sorting, filtering, and pagination, ensuring scalability for real-world data volume.
- Demonstration of full-stack proficiency in REST API design, frontend state management, and database optimization.
