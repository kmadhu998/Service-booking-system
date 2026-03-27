# 🚀 Service Booking System

A full-stack web application built using **Spring Boot, Spring Security, and JWT Authentication** that allows users to securely log in and access protected booking APIs.

---

## 🔥 Features

- 🔐 Secure Login using JWT Authentication  
- 🛡️ Spring Security for API protection  
- 🔑 Password encryption using BCrypt  
- 📦 RESTful APIs for booking management  
- 🌐 Simple frontend (HTML, CSS, JavaScript)  
- ⚡ Stateless authentication (no sessions)  

---

## 🛠️ Tech Stack

- **Backend:** Spring Boot, Spring Security, JWT  
- **Database:** MySQL  
- **Frontend:** HTML, CSS, JavaScript  
- **Build Tool:** Maven  

---

## 🔐 Authentication Flow

1. User logs in with email and password  
2. JWT token is generated upon successful login  
3. Token is stored in browser (localStorage)  
4. Token is sent in `Authorization` header for protected APIs  

---

## 📌 API Endpoints

### 🔓 Public APIs
- `POST /auth/login` → User login  

### 🔒 Protected APIs
- `GET /bookings` → Fetch bookings (Requires JWT Token)  

---

## ⚙️ How to Run the Project

### 🔹 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/service-booking-system.git
cd service-booking-system
spring.datasource.url=jdbc:mysql://localhost:3306/service_db
spring.datasource.username=your_username
spring.datasource.password=your_password

### 🔹 2. Run Backend
```bash
mvn clean install
mvn spring-boot:run
Access Application
http://localhost:8080
