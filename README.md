# User Management API 🚀

A secure and scalable RESTful API built with **Node.js, Express, MongoDB Atlas, and JWT**.

## 🌟 Features
- **User Authentication**: Secure Registration & Login with `bcryptjs` password hashing.
- **Token-based Authorization**: Protected routes using JSON Web Tokens (JWT).
- **Role-Based Access Control (RBAC)**: Distinct permissions for `user` and `admin` roles.
- **Admin Management**: Admins can view all users and delete user accounts.
- **Clean Architecture**: Built following the **MVC** pattern.

## 🛠️ Tech Stack
- **Backend**: Node.js, Express.js
- **Database**: MongoDB Atlas, Mongoose
- **Security**: JSONWebToken (JWT), Bcryptjs

## 🔌 API Endpoints

### Public Routes
- `POST /api/users/register` - Register a new user
- `POST /api/users/login` - Authenticate user & get token

### Protected Routes (User)
- `GET /api/users/profile` - Get logged-in user profile

### Protected Routes (Admin Only)
- `GET /api/users` - Get list of all users
- `DELETE /api/users/:id` - Delete user by ID

## ⚙️ Environment Variables
Create a `.env` file in the root folder and add the following:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key