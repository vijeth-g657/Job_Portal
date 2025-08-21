# Job Portal Application

A full-stack **Job Portal Application** built with the MERN stack (MongoDB, Express.js, React.js, Node.js) that connects recruiters with job seekers.  
Recruiters can post and manage job listings, while candidates can search, apply, and track job applications.

---

## 🚀 Features

### 👩‍💼 For Job Seekers
- User authentication (signup/login with persistent sessions).
- Browse and search job listings with filters.
- Apply for jobs with resume and details.
- Track applied jobs in profile dashboard.

### 🏢 For Recruiters
- Secure recruiter authentication.
- Post, edit, and delete job listings.
- Manage and review applicants.
- Protected recruiter-only routes.

### ⚙️ Core Functionalities
- JWT-based authentication with refresh token support.
- Redux for global state management.
- Persistent sessions using Redux Persist.
- Protected routes using custom `<ProtectedRoute />`.
- Notifications with Sonner Toaster.
- Secure API with Express middleware.
- MongoDB as the database.

---

## 🏗️ Project Architecture

```plaintext
Frontend (React + Redux + Tailwind)
    |
    |--> UI (Job Listings, Profile, Recruiter Dashboard)
    |--> Redux Store (auth, jobs, applications)
    |--> API calls via Axios
    ↓
Backend (Node.js + Express)
    |
    |--> Authentication APIs
    |--> Job Management APIs
    |--> Application Management APIs
    ↓
Database (MongoDB + Mongoose)
    |
    |--> Users (job seekers & recruiters)
    |--> Jobs (posted by recruiters)
    |--> Applications (applied jobs by users)
