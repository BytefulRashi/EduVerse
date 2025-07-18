# 📚 EduVerse – E-Learning Platform

**EduVerse** is a full-stack, real-time e-learning platform where users can browse and purchase courses, manage their cart, join course-based communities, and engage in real-time chat with other learners. The application integrates secure authentication, live messaging, and seamless payments to deliver a robust and interactive learning experience.

---

## 🚀 Features

- 🔐 **Secure Authentication** using Google OAuth and JWT
- 🛒 **Course Purchase & Cart Management** with Razorpay Payment Integration
- 💬 **Real-Time Chat** within course-based communities using Socket.io
- 👥 **User Profile Management** with role-based access
- 📦 **Full E-Commerce Flow** with checkout and order history
- 🧾 **RESTful API backend** using Node.js & Express.js
- 🧠 **MongoDB Database** for storing users, courses, messages, and conversations

---

## 🗂️ Project Structure

```bash
EduVerse/
├── client/                  # React frontend
│   ├── public/              # Static files
│   └── src/                 # React components & entry point
│       ├── components/      # UI components
│       ├── App.js           # Main app
│       ├── index.js         # Entry point
│       └── ...              # Other frontend files
│
├── server/                  # Express backend
│   ├── controllers/         # API controller logic
│   ├── models/              # Mongoose schemas
│   ├── routes/              # API route definitions
│   ├── middlewares/         # Auth/validation logic
│   ├── socket/              # Socket.io server
│   ├── config/              # DB config & env setup
│   ├── index.js             # Backend entry point
│   └── .env                 # Environment variables
│
├── LICENSE
└── README.md
````

---

## 🛠️ Tech Stack

* **Frontend:** React.js, CSS
* **Backend:** Node.js, Express.js
* **Database:** MongoDB with Mongoose
* **Authentication:** JWT + Google OAuth (Google APIs)
* **Real-Time Communication:** Socket.io
* **Payments:** Razorpay API

---

## 🧑‍💻 How to Run the Project Locally

### 1️⃣ Clone the repository

```bash
git clone https://github.com/your-username/EduVerse.git
cd EduVerse
```

---

### 2️⃣ Setup the Backend

```bash
cd server
npm install
```

Create a `.env` file in the `server/` directory and add:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GOOGLE_CLIENT_ID=your_google_client_id
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

Then run the backend server:

```bash
npm start
```

---

### 3️⃣ Setup the Frontend

```bash
cd client
npm install
npm start
```

The React app will run on `http://localhost:3000`

---

## 🧪 Testing

* Frontend: React Testing Library
* Backend: Postman or REST Client (optional)
