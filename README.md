# 🔐 Authentication in Node.js  

🛡️ A lightweight and practical **Node.js Authentication** project built to demonstrate **password hashing** and **JWT-based authentication**. 👨‍💻  

---

## 📝 Problem Statement  
Authentication is a critical aspect of any modern application. Storing plain text passwords is insecure, and access to sensitive routes must be restricted. This project implements:  
- **Task 1:** Secure password storage with **bcrypt hashing**  
- **Task 2:** Token-based authentication with **JWT** for protected routes  

---

## 📊 Features  
- ✅ Task 1: Password Hashing with **bcrypt**  
- ✅ Task 2: JWT Authentication with hashed passwords  
- ✅ Register & Login APIs  
- ✅ Protected route `/profile` with JWT validation  

---

## 💡 Solution / Prototype  
This project:  
- 🔒 Uses **bcrypt** to hash user passwords before storing  
- 🔑 Verifies passwords securely with `bcrypt.compare`  
- 🪪 Generates **JWT tokens** upon successful login  
- 🚪 Restricts access to protected routes unless a valid token is provided  

---

## 🛠️ Technologies & Tools Used  
- 🌐 **Node.js + Express** – Backend framework  
- 🔑 **bcrypt** – Password hashing  
- 🪙 **jsonwebtoken (JWT)** – Authentication tokens  
- 📦 **body-parser** – JSON request parsing  

---

## 📸 API Endpoints  

### Task 1 – Password Hashing Authentication  
- `POST /register` → Register user (store hashed password)  
- `POST /login` → Login with password verification  

### Task 2 – JWT Authentication (with Hashing)  
- `POST /register` → Register user (hashed password)  
- `POST /login` → Login and receive JWT  
- `GET /profile` → Protected route (requires valid JWT)  

---

## ⚙️ How to Run the Project  

1. 📥 **Clone the repository**  
   ```bash
   git clone https://github.com/Smasher5/auth-assignment.git
   cd auth-assignment
