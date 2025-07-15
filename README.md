# 🗳️ Voting Application

This is a backend application for a voting system where users can vote for candidates.  
It provides functionalities for **user authentication**, **candidate management**, and **voting**.

---

## 🚀 Features

✅ User sign up and login with **Aadhar Card Number** and **password**  
✅ User can view the list of candidates  
✅ User can vote for a candidate (**only once**)  
✅ Admin can manage candidates (**add, update, delete**)  
🚫 Admin cannot vote  

---

## 🛠️ Technologies Used

- Node.js
- Express.js
- MongoDB
- JSON Web Tokens (JWT) for authentication

---

## 📚 API Endpoints

### 🔐 Authentication

- **Sign Up**  
  `POST /signup` — Sign up a user

- **Login**  
  `POST /login` — Login a user

---

### 🗳️ Candidates

- **Get Candidates**  
  `GET /candidates` — Get the list of candidates

- **Add Candidate** (Admin only)  
  `POST /candidates` — Add a new candidate

- **Update Candidate** (Admin only)  
  `PUT /candidates/:id` — Update a candidate by ID

- **Delete Candidate** (Admin only)  
  `DELETE /candidates/:id` — Delete a candidate by ID

---

### 🗳️ Voting

- **Get Vote Count**  
  `GET /candidates/vote/count` — Get the count of votes for each candidate

- **Vote for Candidate** (User only)  
  `POST /candidates/vote/:id` — Vote for a candidate (only once)

---

### 👤 User Profile

- **Get Profile**  
  `GET /users/profile` — Get user profile information

- **Change Password**  
  `PUT /users/profile/password` — Change user password

---

## 📦 Setup Instructions

1️⃣ **Clone the repository:**
```bash
git clone https://github.com/ashu4040/Voting_App.git
cd voting-application

2️⃣ Install dependencies:
npm install

3️⃣ Create a .env file and add your environment variables:
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000

4️⃣ Run the server:
npm start
Server will start on:
🌐 http://localhost:5000
