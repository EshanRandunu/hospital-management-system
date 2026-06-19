# 🏥 MediLink - AI-Enabled Smart Healthcare Appointment & Telemedicine Platform

A cloud-native healthcare management platform developed for the **SE3020 - Distributed Systems** module. The system follows a **Microservices Architecture** and enables patients, doctors, and administrators to manage healthcare services efficiently through a secure web application.

---

## 📖 Project Overview

MediLink is a distributed healthcare platform inspired by modern telemedicine systems. It provides appointment booking, patient management, doctor management, digital prescriptions, and secure authentication using independent microservices.

The application was developed using Spring Boot, React, MongoDB, Docker, and JWT Authentication.

---

## 🚀 Features

### 👤 Patient

- Register and Login
- Manage Profile
- Browse Available Doctors
- Search Doctors by Specialty
- Book Appointments
- View Appointment History
- Upload Medical Reports
- View Uploaded Reports

### 👨‍⚕️ Doctor

- Secure Login
- Manage Doctor Profile
- Set Availability
- Accept or Reject Appointment Requests
- View Patient Medical Reports
- Issue Digital Prescriptions
- View Scheduled Appointments

### 👨‍💼 Administrator

- Admin Authentication
- Manage Patients
- Manage Doctors
- Verify Doctor Registrations
- Monitor Platform Users

---

## 🏗 System Architecture

The project follows a **Microservices Architecture**.

### Services

- Authentication Service
- Patient Service
- Doctor Service
- Appointment Service
- API Gateway

Each service maintains its own business logic and communicates through REST APIs.

---

## 🛠 Technology Stack

### Backend

- Java 17
- Spring Boot
- Spring Security
- JWT Authentication
- Spring Data MongoDB
- Maven

### Frontend

- React.js
- Axios
- React Router
- Bootstrap / CSS

### Database

- MongoDB

### DevOps

- Docker
- Docker Compose

### Version Control

- Git
- GitHub

---

## 🔐 Authentication

The application uses **JWT (JSON Web Tokens)** for secure authentication and authorization.

Supported Roles:

- Patient
- Doctor
- Admin

Role-based access control is implemented for protected endpoints.

---

## 📂 Project Structure

```
hospital-management-system
│
├── backend
│   ├── auth-service
│   ├── patient-service
│   ├── doctor-service
│   ├── appointment-service
│   ├── api-gateway
│   └── ...
│
├── frontend
│
├── docker-compose.yml
│
└── README.md
```

---

# ⚙ Installation

## Prerequisites

- Java 17+
- Node.js
- MongoDB
- Maven
- Docker (Optional)

---

## Backend Setup

1. Navigate to the backend directory.

```
cd backend
```

2. Create the configuration file.

```
application.properties
```

from

```
application-template.properties
```

3. Configure the following properties.

```
MONGO_URI=
JWT_SECRET=
ADMIN_PASSWORD=
```

4. Run the backend.

```
./mvnw spring-boot:run
```

or

```
mvn spring-boot:run
```

---

## Frontend Setup

Navigate to the frontend directory.

```
cd frontend
```

Install dependencies.

```
npm install
```

Create a `.env` file.

```
REACT_APP_API_URL=http://localhost:8080
```

Run the application.

```
npm start
```

---

## 🐳 Docker

Build and start all services.

```
docker-compose up --build
```

---

## 📡 REST APIs

Example endpoints:

### Authentication

```
POST /auth/register
POST /auth/login
```

### Patient

```
GET /patients
PUT /patients/{id}
POST /patients/upload-report
```

### Doctor

```
GET /doctors
PUT /doctors/profile
POST /doctors/prescription
```

### Appointment

```
POST /appointments
GET /appointments
PUT /appointments/{id}
DELETE /appointments/{id}
```

---

## ✅ Implemented Features

✔ JWT Authentication

✔ Role-Based Authorization

✔ Patient Management

✔ Doctor Management

✔ Appointment Booking

✔ Medical Report Upload

✔ Digital Prescriptions

✔ RESTful APIs

✔ MongoDB Integration

✔ Docker Containerization

✔ Responsive React Frontend

---

## 🚧 Features Not Implemented

The following features mentioned in the assignment specification were not implemented in this version:

- Video Consultation Integration
- Online Payment Gateway
- SMS Notifications
- Email Notifications
- AI Symptom Checker

---

## 👨‍💻 Team

- Thisantha Edirisingha
- Eshan Randunu
- Nawoda Hasaranga
- Ayesh Arachchige

Developed as a group project for

**SE3020 - Distributed Systems**

BSc (Hons) Information Technology Specializing in Software Engineering

SLIIT

---

## 📄 License

This project was developed for academic purposes only.
