# MERN CRUD User Management App

This is a full-stack user management application built using the MERN stack (MongoDB, Express.js, React.js, Node.js). It allows users to perform basic CRUD operations: Create, Read, Update, and Delete user records.

✨ Features

- ✅ Add New User
- 📋 View All Users
- ✏️ Edit/Update Existing User
- 🗑️ Delete User
- 📦 RESTful API built with Express.js and MongoDB
- ⚛️ Frontend using React with React Router

📁 Folder Structure

```
MERN-CRUD/
├── client/                 # React frontend
│   ├── src/
│   │   ├── adduser/        # AddUser component
│   │   ├── getuser/        # User listing component
│   │   ├── updateuser/     # UpdateUser component
│   │   ├── App.js
│   │   └── index.js
│   └── public/
│
├── server/                 # Node + Express backend
│   ├── controller/         # Controller logic
│   │   └── userController.js
│   ├── model/              # Mongoose schema
│   │   └── userModel.js
│   ├── routes/             # API routes
│   │   └── userRoute.js
│   ├── .env                # Environment variables
│   └── index.js            # Entry point
│
├── package.json            # Backend dependencies
└── README.md
```

🔧 Installation & Setup

1. Clone the repo:

```bash
git clone https://github.com/your-username/mern-crud-app.git
cd mern-crud-app
```

2. Install server dependencies:

```bash
cd server
npm install
```

3. Install client dependencies:

```bash
cd ../client
npm install
```

4. Create a .env file in /server:

```env
PORT=8000
MONGO_URI=your_mongodb_connection_string
```

5. Run both servers:

Start the backend:

```bash
cd server
npm run dev
```

Start the frontend:

```bash
cd ../client
npm start
```

🌐 App will run on:

- Frontend: http://localhost:3000
- Backend: http://localhost:8000

🔁 CRUD Operations Summary

| Operation | Route                     | Method | Description            |
|----------|---------------------------|--------|------------------------|
| Create   | /api/user                 | POST   | Add a new user         |
| Read     | /api/users                | GET    | Get all users          |
| Read     | /api/user/:id             | GET    | Get user by ID         |
| Update   | /api/update/user/:id      | PUT    | Update user by ID      |
| Delete   | /api/delete/user/:id      | DELETE | Delete user by ID      |

📦 Dependencies

Client (React)

- axios
- react
- react-dom
- react-router-dom
- react-hot-toast
- bootstrap
- font-awesome

Server (Node + Express)

- express
- mongoose
- dotenv
- cors

💡 Dev Dependencies

- nodemon (for backend hot-reload)

📸 UI Highlights

- Toast notifications for feedback
- Bootstrap + FontAwesome for styling
- Clean and minimal UX
