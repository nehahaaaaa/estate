Welcome to the *Commercial Real Estate Auth System* project! This web application allows users to register, log in, and access a homepage using a simple authentication system. The project implements *Node.js, **Express, **MongoDB, and **JWT* for user authentication. Users' passwords are securely stored using *bcryptjs, and authentication is handled via **JWT tokens*.

---

## 🚀 Features

- 📝 *User Registration*: New users can register securely.
- 🔒 *User Login*: Registered users can log in and receive a JWT token.
- 🏠 *Homepage Access*: Upon login, users are redirected to the homepage.
- 🔐 *JWT Authentication*: Secure token-based authentication.
- 💾 *MongoDB Integration*: User data is stored in MongoDB.
- 💼 *Password Hashing*: Passwords are securely hashed using bcryptjs.

---

## 🛠️ Tech Stack

- *Backend*: 
  - Node.js
  - Express.js
  - MongoDB (Mongoose for ORM)
  - JWT (JsonWebToken) for secure authentication
  - bcryptjs for password hashing

- *Frontend*:
  - HTML, CSS, JavaScript (Vanilla)

---

## 📦 Dependencies

Make sure you have the following packages installed:

json
"bcryptjs": "^2.4.3",
"body-parser": "^1.20.3",
"cors": "^2.8.5",
"dotenv": "^16.4.5",
"express": "^4.21.0",
"jsonwebtoken": "^9.0.2",
"mongodb": "^6.9.0",
"mongoose": "^8.6.2"

## Install Dependencies
bash
npm install

## Setup Environment Variables

PORT=8000
JWT_SECRET=your_jwt_secret_key
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/realestate?retryWrites=true&w=majority

## Start the Server
npm start

- The server will start at http://localhost:8000.

## 🗄️ MongoDB Integration
The application uses MongoDB as its database to store user information. Make sure you have MongoDB set up and running, and your .env file is properly configured with the MongoDB connection string.

## 📜 Middleware
This project includes an authentication middleware to protect routes using JWT. You can easily secure any route by adding the middleware to it.

## 🌐 Frontend
- The frontend consists of Login, Register, and Home pages.
- Login and Register Pages: Users can sign up and log in. Upon successful login, the user is redirected to the Home page.
- LocalStorage: Upon successful login, the user’s JWT token is stored in localStorage for future authenticated requests.

## 🚀 Deployment
You can easily deploy this project to services like Heroku, Vercel, or any other cloud provider. Ensure that your MongoDB database is accessible via a remote URI (like MongoDB Atlas) and that you configure your environment variables properly.

## 🛡️ Security
- Passwords are hashed using bcryptjs before storing them in the database.
- JWT tokens are used for secure session management.
- Ensure you use strong environment variables and keep your JWT_SECRET safe
