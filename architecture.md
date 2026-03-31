# System Architecture
## JobPortal - Online Recruitment System

---

## 1. Overview

JobPortal is a web-based recruitment platform that connects job seekers and employers.

Tech stack:
- Backend: Django
- Frontend: HTML, CSS, JavaScript, Bootstrap
- Database: PostgreSQL

---

## 2. Architecture Pattern

- MVC (Model - View - Template)
- Client-Server Architecture

---

## 3. High-Level Architecture

Client (Browser)
    ↓
Frontend (HTML + Bootstrap + JS)
    ↓
Django Views (Controller)
    ↓
Django Models (ORM)
    ↓
PostgreSQL Database

---

## 4. Components

### 4.1 Frontend Layer
- Render UI
- Handle user interaction
- Send HTTP requests (Fetch API)

### 4.2 Backend Layer (Django)
- Authentication
- Business logic
- API endpoints
- Data validation

### 4.3 Database Layer
- Store users, jobs, applications, resumes

---

## 5. Core Modules

- accounts (authentication, profile)
- jobs (job, company)
- applications (apply, resume)

---

## 6. Data Flow

1. User sends request from browser
2. Frontend sends request to backend
3. Backend processes logic
4. Query PostgreSQL
5. Return response

---

## 7. Security

- Django authentication
- Password hashing
- CSRF protection
- Role-based access

---

## 8. Scalability

- Upgrade to REST API
- Integrate React (future)
- Add caching

---