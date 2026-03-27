# SYSTEM REQUIREMENTS
## Online Recruitment Website

---

## 1. Introduction

This document defines the functional and non-functional requirements for the recruitment website.

---

## 2. User Roles

### 2.1 Guest
- View jobs
- Search jobs

### 2.2 Job Seeker
- Register / Login
- Create profile
- Upload CV
- Apply for jobs

### 2.3 Employer
- Register / Login
- Post jobs
- Manage applications

### 2.4 Admin
- Manage users
- Manage jobs
- System control

---

## 3. Functional Requirements

---

### 3.1 Authentication System

- User registration
- User login/logout
- Password encryption
- Role selection (Seeker / Employer)

---

### 3.2 User Profile

#### Job Seeker:
- Name, email, phone
- Skills
- Experience
- Education

#### Employer:
- Company name
- Description
- Address

---

### 3.3 Job Management

Employer can:
- Create job
- Edit job
- Delete job
- View applicants

Job includes:
- Title
- Description
- Salary
- Location
- Requirements

---

### 3.4 Job Search

- Search by keyword
- Filter by:
  - Salary
  - Location
  - Job type

---

### 3.5 CV Management

- Upload CV (PDF)
- Edit CV info
- Delete CV

---

### 3.6 Job Application

- Apply to job
- Save job
- Track application status

Status:
- Pending
- Accepted
- Rejected

---

### 3.7 Admin Dashboard

- View all users
- Delete users
- Manage job posts
- View system statistics

---

## 4. Non-Functional Requirements

---

### 4.1 Performance
- Page load < 3 seconds
- Handle 1000+ users

---

### 4.2 Security
- Password hashing
- CSRF protection
- SQL injection prevention

---

### 4.3 Usability
- Simple UI
- Mobile responsive

---

### 4.4 Reliability
- System uptime 99%
- Backup database

---

### 4.5 Scalability
- Support future expansion
- Easy API integration

---

## 5. Database Requirements

### Tables:

#### users
- id
- username
- password
- role

#### profiles
- user_id
- name
- phone
- address

#### jobs
- id
- employer_id
- title
- description
- salary

#### applications
- id
- job_id
- user_id
- status

#### resumes
- id
- user_id
- file_path

---

## 6. API Requirements

Examples:

- POST /register
- POST /login
- GET /jobs
- POST /apply
- GET /applications

---

## 7. Constraints

- Use Django framework
- Use PostgreSQL database
- Frontend must use HTML/CSS/JS

---

## 8. Timeline (2 months)

Week 1-2:
- Setup project
- Database design

Week 3-4:
- Authentication
- User profile

Week 5-6:
- Job + Apply system

Week 7:
- Admin + Testing

Week 8:
- Deployment + Report

---

## 9. Success Criteria

- Fully working system
- Clean UI
- Data stored correctly
- No major bugs

---