# 🎓 RecruitAi — AI-Powered Campus Recruitment System

![Live](https://img.shields.io/badge/Live-Online-brightgreen)
![Java](https://img.shields.io/badge/Java-17-orange)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.0-green)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)

> A full-stack campus placement platform that automates the entire recruitment process — from student registration to final selection.

## 🔗 Live Demo
### **[➡️ https://recruitai-pu35.onrender.com](https://recruitai-pu35.onrender.com)**

---

## 🚀 The Problem It Solves

Traditional campus placement is slow, manual and error-prone:
- ❌ Spreadsheets and paper forms
- ❌ Students unaware of their application status
- ❌ No automated student-job matching
- ❌ Recruiter verification takes days

RecruitAi solves all of this with one unified digital platform.

---

## ✨ Key Features

### ⚡ Auto-Shortlisting
The moment a recruiter posts a job, the system instantly scans all students and shortlists eligible ones based on CGPA, branch and skills — no manual work needed.

### 🔐 Secure Authentication
JWT-based stateless authentication with BCrypt password hashing and Spring Security role-based access control.

### 📊 Real-Time Tracking
Students track their application status live: Applied → Shortlisted → Interview → Selected

### 🏛️ Recruiter Approval Workflow
New recruiters start as PENDING. College admin reviews and approves or rejects — maintaining campus security.

### 📝 Coding Tests
Recruiters create MCQ-based coding tests. Students attempt them. Results visible instantly to recruiters.

### 📈 Placement Analytics
Admin dashboard with live stats — total placed, branch-wise reports, active recruiters.

---

## 👥 Three Role-Based Portals

| Role | Key Actions |
|------|-------------|
| 🎓 Student | Browse jobs, get auto-shortlisted, track application status |
| 🏢 Recruiter | Post jobs, manage candidates, create coding tests |
| 🏛️ College Admin | Approve recruiters, manage students, view analytics |

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|-------------|
| Frontend | HTML5, CSS3, Vanilla JavaScript, Fetch API |
| Backend | Java 17, Spring Boot 3, Spring Security, Hibernate |
| Auth | JWT (RFC 7519), BCrypt |
| Database | MySQL 8 on Aiven Cloud |
| Hosting | Render.com with GitHub auto-deploy |

---

## 🗄️ Database — 8 Tables

| Table | Purpose |
|-------|---------|
| users | All 3 user types with role column |
| student_profiles | CGPA, branch, skills, resume URL |
| recruiter_profiles | Company name, approval status |
| job_postings | Job details and eligibility criteria |
| applications | Student-job mapping with status |
| coding_tests | Recruiter-created MCQ tests |
| notifications | Status change alerts |
| courses | Learning resources for students |

---

## 🔒 Security

- JWT tokens expire after 24 hours
- Each role can only access its own endpoints
- Passwords stored as BCrypt hashes — never plain text
- College admin controls who can recruit on campus

---

## 🌐 Key API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/login | Login and get JWT token |
| POST | /api/auth/register | Register new user |
| GET | /api/student/jobs | Browse all active jobs |
| POST | /api/student/jobs/{id}/apply | Apply for a job |
| POST | /api/recruiter/jobs | Post job — triggers auto-shortlist |
| PUT | /api/recruiter/applications/{id}/status | Update candidate status |
| PUT | /api/admin/recruiters/{id}/approve | Approve a recruiter |
| GET | /api/admin/stats | View placement analytics |

---

## 📁 Frontend Files

| File | Purpose |
|------|---------|
| index.html | Login page |
| register.html | Registration with role selection |
| student-dashboard.html | Student portal |
| recruiter-dashboard.html | Recruiter portal |
| admin-dashboard.html | Admin portal |

---


## 👥 Team

| Member | GitHub |
|---|---|
| Shanti Priya | [@ShantiPr28-byte](https://github.com/ShantiPr28-byte) |
| Shashank Rai | [@Shashankrai30](https://github.com/Shashankrai30) |

---

## 📄 License

This project is licensed under the MIT License.

---

Made with ❤️ for Campus Placement Management
