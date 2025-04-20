# MERN Stack CRUD App (User Management App)

This is a full-stack user management application built with the MERN stack. It allows you to Create, Read, Update, and Delete (CRUD) users through a web interface.

## 🛠️ Tech Stack

- MongoDB – NoSQL database
- Express.js – Node.js web framework
- React.js – Frontend library
- Node.js – Backend runtime environment

## 📁 Folder Structure

```
MERN-CRUD-App/
│
├── client/                 # React frontend
│   ├── src/
│   │   ├── adduser/        # Add user component
│   │   ├── getuser/        # User list view
│   │   ├── updateuser/     # Update user form
│   │   ├── App.js          # Route configuration
│   │   └── index.js        # Entry point for React app
│   ├── public/
│   └── package.json        # Frontend dependencies
│
├── server/                 # Node.js + Express backend
│   ├── controller/         # Logic for each API route
│   ├── model/              # Mongoose schema
│   ├── routes/             # Express routes
│   ├── index.js            # Entry point for backend server
│   └── .env                # Environment variables
│
├── package.json            # Project-level metadata
└── README.md               # Project overview (you’re here!)
```

## 🔧 Features

- Create new users
- Display list of users
- Update user details
- Delete users
- Toast notifications for user feedback

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/mern-user-management.git
cd mern-user-management
```

### 2. Set Up the Backend

```bash
cd server
npm install
```

Create a `.env` file in the server directory:

```
PORT=8000
MONGO_URI=mongodb://localhost:27017/mern_user_crud
```

Start the backend server:

```bash
npm start
```

### 3. Set Up the Frontend

```bash
cd client
npm install
npm start
```

The React app will run on `http://localhost:3000` and connect to the backend at `http://localhost:8000`.

## 🖼️ UI Preview

- Add User Page
- View All Users Table
- Update User Page
- Delete confirmation via Toast

(You can add screenshots here if desired.)

## 📬 API Endpoints

| Method | Endpoint                 | Description           |
|--------|--------------------------|-----------------------|
| POST   | /api/user                | Create a new user     |
| GET    | /api/users               | Get all users         |
| GET    | /api/user/:id            | Get user by ID        |
| PUT    | /api/update/user/:id     | Update user by ID     |
| DELETE | /api/delete/user/:id     | Delete user by ID     |

## ✨ Dependencies Highlights

Frontend:

- axios
- react-router-dom
- react-hot-toast
- font-awesome

Backend:

- express
- mongoose
- dotenv
- cors

## 💡 Future Improvements

- Form validation
- Pagination & search
- Responsive design
- User authentication
