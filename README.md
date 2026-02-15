# 🔐 Secure User Authentication System (Task-01)

## 📌 Project Overview

This project is a Full Stack Secure Authentication System developed as part of the Prodigy Infotech Internship – Task 01.

The system allows users to:
- Register a new account
- Login securely
- Access protected routes only after authentication
- Logout securely

The application follows secure authentication practices including password hashing and JWT-based authorization.

---

## 🚀 Tech Stack

### Backend
- Node.js
- Express.js
- MySQL
- bcrypt (Password Hashing)
- JSON Web Token (JWT)
- dotenv

### Frontend
- HTML
- CSS
- JavaScript (Fetch API)

---

## 🔐 Key Features

- User Registration  
- Secure Password Hashing using bcrypt  
- JWT Token Generation  
- Protected Routes using Middleware  
- Token Expiry Handling  
- Logout Functionality  
- Clean Project Structure  
- Environment Variable Protection  

---

## 📂 Project Structure

PRODIGY_FS_01
│
├── server/
│ ├── middleware/
│ ├── routes/
│ ├── db.js
│ ├── server.js
│ ├── package.json
│ └── package-lock.json
│
├── frontend/
│ ├── login.html
│ ├── register.html
│ ├── dashboard.html
│ └── style.css
│
├── .gitignore
├── README.md
└── LICENSE


---

## ⚙️ Installation & Setup Guide

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/Claraxavi/PRODIGY_FS_01.git
cd PRODIGY_FS_01

2️⃣ Install Backend Dependencies
cd server
npm install

3️⃣ Create Environment File

Inside the server folder, create a file named .env and add:

PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=prodigy_auth
JWT_SECRET=your_secret_key

4️⃣ Start the Server
npm start


Server will run at:

http://localhost:5000

5️⃣ Run Frontend

Open frontend/login.html using Live Server in VS Code.

🔄 Authentication Flow

1.User registers an account

2.Password is hashed using bcrypt

3.User logs in

4.JWT token is generated

5.Token is stored in browser localStorage

6.Protected routes verify the token using middleware

7.Logout removes the token from storage

🛡 Security Implementation

Passwords are hashed before storing in the database

JWT tokens are signed using a secret key

Protected routes require valid authentication tokens

Sensitive credentials are stored in .env file

.env and node_modules are ignored via .gitignore

📜 License

This project is licensed under the MIT License.


