# SYSTEM ARCHITECTURE
## Online Recruitment Website (Django + JavaScript)

---

## 1. Overview

This system is a web-based recruitment platform that connects job seekers and employers.

- Backend: Django (Python)
- Frontend: HTML, CSS, JavaScript
- Database: PostgreSQL
- Architecture: Client - Server (MVC Pattern)

---

## 2. High-Level Architecture

[Client - Browser]
        |
        v
[Frontend - HTML/CSS/JS]
        |
        v
[Backend - Django REST / Views]
        |
        v
[Database - PostgreSQL]

---

## 3. Components

### 3.1 Frontend Layer
- Technologies: HTML5, CSS3, JavaScript
- Responsibilities:
  - Render UI
  - Handle user interactions
  - Call backend APIs (AJAX / Fetch)

---

### 3.2 Backend Layer (Django)

Modules:
- Authentication (Login/Register)
- Job Management
- CV Management
- Application Processing
- Admin Panel

Responsibilities:
- Business logic
- API endpoints
- Data validation
- Security

---

### 3.3 Database Layer (PostgreSQL)

Main Tables:
- users
- profiles
- jobs
- applications
- resumes

---

## 4. Architecture Pattern

- MVC Pattern (Model - View - Template)
- RESTful API design (optional with Django REST Framework)

---

## 5. Data Flow

1. User sends request (login, search job)
2. Frontend sends API request to backend
3. Backend processes logic
4. Query database
5. Return JSON / HTML response
6. Frontend updates UI

---

## 6. Deployment Architecture

- Web Server: Nginx
- App Server: Gunicorn
- Database: PostgreSQL
- Hosting: VPS / Cloud (AWS, DigitalOcean)

---

## 7. Security

- Authentication: Django Auth
- Password hashing
- CSRF protection
- Input validation
- Role-based access control

---

## 8. Scalability

- Use PostgreSQL indexing
- Separate frontend/backend (future: React)
- Caching (Redis - optional)

---

## 9. Future Improvements

- AI job recommendation
- Chat system (Employer - Candidate)
- Email notifications
- Resume parsing

---