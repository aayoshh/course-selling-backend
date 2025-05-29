# 📚 Course Selling Backend API

This is the backend service for a course-selling platform. It supports user registration and login, course creation and management by admins, and course browsing and purchasing by users.

---

## 🛠️ Tech Stack

- Node.js / Express.js (assumed)
- MongoDB / Mongoose (assumed)
- RESTful API structure
- JWT Authentication (assumed)

---

## 📌 API Endpoints

### 👤 User Routes (`/api/v1/user`)

| Method | Endpoint                  | Description              |
|--------|---------------------------|--------------------------|
| POST   | `/signup`                 | Register a new user      |
| POST   | `/signin`                 | Login a user             |
| GET    | `/purchases`              | Get all user purchases   |

---

### 🔐 Admin Routes (`/api/v1/admin`)

| Method | Endpoint                  | Description                       |
|--------|---------------------------|-----------------------------------|
| POST   | `/signup`                 | Register a new admin              |
| POST   | `/signin`                 | Login as admin                    |
| POST   | `/course`                 | Create a new course               |
| PUT    | `/course/:id`            | Update an existing course         |
| DELETE | `/course/:id`            | Delete a course                   |
| GET    | `/course/view-all`       | View all courses (admin access)   |

---

### 📦 Course Routes (`/api/v1/course`)

| Method | Endpoint         | Description                    |
|--------|------------------|--------------------------------|
| POST   | `/purchase`      | Purchase a course              |
| GET    | `/preview`       | Preview available courses      |

---

## ✅ Features

- User and Admin authentication
- Role-based access control
- Course management by Admins
- Course purchase and preview by Users

---

## 🔐 Authentication

Authentication is handled via JWTs. Include the token in the `Authorization` header as:

