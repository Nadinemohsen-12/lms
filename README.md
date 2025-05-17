# lms
# Learning Platform

A full-stack web application for managing and delivering online courses. This platform provides features for both students and administrators to manage course content, enrollments, and user interactions.

## Features

- 🔐 User Authentication (Login/Register)
- 👥 User Roles (Admin/Student)
- 📚 Course Management
- 🛒 Shopping Cart Functionality
- 👤 User Profile Management
- 📊 Admin Dashboard
- 🎓 Course Enrollment System

## Tech Stack

### Frontend
- React.js
- Redux for state management
- Material-UI (MUI) for UI components
- React Router for navigation

### Backend
- Node.js
- Express.js
- MongoDB (Database)
- JWT for authentication

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher)


## Installation

1. Clone the repository:
```bash
git clone https://github.com/Nadinemohsen-12/lms.git
```

2. Install backend dependencies:
```bash
cd backend
npm install
```

3. Install frontend dependencies:
```bash
cd frontend
npm install
```

## Environment Variables

Create `.env` files in both frontend and backend directories:

### Backend `.env`:
```
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### Frontend `.env`:
```
REACT_APP_API_URL=http://localhost:5000/api
```

## Running the Application

1. Start the backend server:
```bash
cd backend
npm run dev
```

2. Start the frontend development server:
```bash
cd frontend
npm start
```

The application will be available at `http://localhost:3000`

## Project Structure

```
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── features/
│   │   ├── pages/
│   │   └── App.js
│   └── package.json
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── server.js
└── README.md
```

## API Endpoints

### Auth Routes
- POST `/api/auth/register` - Register new user
- POST `/api/auth/login` - User login

### Course Routes
- GET `/api/courses` - Get all courses
- GET `/api/courses/:id` - Get specific course
- POST `/api/courses` - Create new course (Admin only)
- PUT `/api/courses/:id` - Update course (Admin only)
- DELETE `/api/courses/:id` - Delete course (Admin only)

### User Routes
- GET `/api/users/profile` - Get user profile
- PUT `/api/users/profile` - Update user profile

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, please email [support@email.com] or open an issue in the repository. 
