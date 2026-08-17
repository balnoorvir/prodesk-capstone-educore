
# EduCore — Enterprise Learning Management System

## Project Overview

**Project Name:** EduCore
**Project Type:** Enterprise Learning Management System (LMS)
**Capstone Phase:** Sprint 13
**Development Duration:** 4 Weeks

### Objective

EduCore is an enterprise-level Learning Management System designed to provide a centralized platform for students, instructors, and administrators.

The platform will allow students to access courses, lessons, assignments, quizzes, grades, and learning progress. Instructors will be able to create and manage educational content, assignments, quizzes, and student performance. Administrators will manage users, courses, and overall platform activity.

---

## User Roles

### Student

Students can:

* Register and log in
* Browse available courses
* Enroll in courses
* View enrolled courses
* Access lessons
* Mark lessons as completed
* Track learning progress
* View and submit assignments
* Attempt quizzes
* View grades and quiz results
* Receive notifications

### Instructor

Instructors can:

* Log in
* Create and manage courses
* Add, edit, and delete lessons
* Create assignments
* Review student submissions
* Grade assignments
* Create quizzes
* View enrolled students
* Monitor course performance

### Administrator

Administrators can:

* Manage users
* Manage students and instructors
* Manage courses
* Activate or deactivate accounts
* View platform statistics
* Monitor overall system activity

---

## Core Functional Requirements

### 1. Authentication

The system will provide:

* User registration
* User login
* Logout
* Password validation
* Role identification
* Protected routes
* Role-based authorization

Users will only be able to access features permitted for their assigned role.

### 2. Student Dashboard

The student dashboard will display:

* Enrolled courses
* Overall learning progress
* Upcoming assignments
* Recent activity
* Recent grades
* Notifications

### 3. Course Management

Students can:

* Browse courses
* Search courses
* View course details
* Enroll in courses
* Access enrolled courses

Instructors can:

* Create courses
* Edit courses
* Delete their courses
* Add and manage lessons

Administrators can:

* View all courses
* Manage courses
* Control course availability

### 4. Learning Management

Courses will contain modules and lessons.

Students will be able to:

* Open lessons
* Mark lessons as completed
* Continue from previous progress
* View course completion percentage

### 5. Assignment Management

Students can:

* View assignments
* View deadlines
* Read instructions
* Submit assignments
* View grades

Instructors can:

* Create assignments
* Set deadlines
* Add descriptions
* View submissions
* Grade submissions

### 6. Quiz Management

Students can:

* Start quizzes
* Answer questions
* Submit quizzes
* View quiz results

Instructors can:

* Create quizzes
* Add questions
* Add multiple-choice options
* Define correct answers
* View student results

### 7. Grade Management

Students can view:

* Assignment scores
* Quiz scores
* Course performance
* Overall grades

Instructors can:

* Enter assignment grades
* Review student performance
* View course-level performance

### 8. Notifications

The system may provide notifications for:

* New assignments
* Upcoming deadlines
* Assignment grading
* New courses
* Quiz availability

### 9. Analytics

Student analytics may include:

* Course completion
* Quiz performance
* Assignment performance
* Overall progress

Instructor analytics may include:

* Number of enrolled students
* Average scores
* Course completion rate
* Pending submissions

Administrator analytics may include:

* Total users
* Total students
* Total instructors
* Total courses
* Platform activity

---

# Feature Prioritization

## P0 — Mandatory MVP

The following features form the minimum viable product:

* User authentication
* Role-based authorization
* Student dashboard
* Instructor dashboard
* Admin dashboard
* Course management
* Course enrollment
* Lessons
* Learning progress tracking
* Assignments
* Assignment submission
* Assignment grading
* Quizzes
* Quiz results
* Grades
* Basic user management

## P1 — Priority Features

* Course search
* Course filtering
* Notifications
* Calendar
* Student analytics
* Instructor analytics
* Improved admin analytics

## P2 — Stretch Goals

* AI learning assistant
* AI-based course recommendations
* Advanced analytics
* Real-time notifications
* Personalized learning suggestions

---

# Technology Stack

## Frontend

* React
* JavaScript
* Vite
* Redux Toolkit
* CSS

## Backend

* Node.js
* Express.js

## Database

* MongoDB

## API

* REST API

## Authentication

* JWT-based authentication

## UI/UX Design

* Figma

## System Architecture

* Draw.io

## Version Control

* Git
* GitHub

## Deployment

* Vercel for frontend
* MongoDB Atlas for database
* Backend deployment platform to be finalized during implementation

---

# Database Requirements

EduCore will use MongoDB as its database.

Initial collections will include:

* `users`
* `courses`
* `lessons`
* `enrollments`
* `assignments`
* `submissions`
* `quizzes`
* `questions`
* `quiz_results`
* `notifications`

The final database structure and relationships will be represented through an Entity Relationship Diagram (ERD).

---

# Frontend State Management

Redux Toolkit will be used to manage global application state.

The planned Redux state tree includes:

```text
Redux Store
│
├── auth
├── courses
├── lessons
├── assignments
├── quizzes
├── progress
├── grades
├── notifications
└── ui
```

The state structure may be refined during implementation based on application requirements.

---

# API Requirements

EduCore will use REST APIs for communication between the frontend and backend.

Initial planned endpoints include:

```text
POST   /api/auth/register
POST   /api/auth/login
POST   /api/auth/logout

GET    /api/courses
POST   /api/courses
GET    /api/courses/:id
PUT    /api/courses/:id
DELETE /api/courses/:id

GET    /api/courses/:id/lessons
POST   /api/courses/:id/lessons

GET    /api/assignments
POST   /api/assignments
POST   /api/assignments/:id/submit

GET    /api/quizzes
POST   /api/quizzes
POST   /api/quizzes/:id/submit

GET    /api/grades
GET    /api/notifications
```

These endpoints represent the planned API architecture and will be implemented during the development phase.

---

# UI/UX Requirements

Figma will be used to design the EduCore interface before implementation.

## Minimum Required Screens

1. Authentication Screen
2. Main Dashboard
3. Course Details / Data Details View

## Additional Planned Screens

4. Instructor Dashboard
5. Assignment Details
6. Admin Dashboard

The final Figma file will contain the application's UI designs and relevant user flows.

**Figma Design:** To be added after completion.

---

# System Architecture

The planned system architecture is:

```text
                    USER
                      │
                      ▼
              ┌──────────────┐
              │   FRONTEND   │
              │ React + Vite │
              │ Redux Toolkit│
              └──────┬───────┘
                     │
                  REST API
                     │
                     ▼
              ┌──────────────┐
              │   BACKEND    │
              │Node.js +     │
              │Express.js    │
              └──────┬───────┘
                     │
                     ▼
              ┌──────────────┐
              │   MongoDB    │
              │   Database   │
              └──────────────┘
```

A detailed system architecture diagram and MongoDB ERD will be created during the architecture phase.

---

# Security Requirements

EduCore will implement:

* Password protection
* JWT authentication
* Protected routes
* Role-based authorization
* Input validation
* Secure API requests
* Prevention of unauthorized access

For example:

```text
Student → /admin/users → Access Denied

Admin → /admin/users → Access Granted
```

---

# Responsive Design

The application will be designed to work across:

* Desktop
* Laptop
* Tablet
* Mobile

The Figma designs will primarily focus on desktop layouts while maintaining responsive design considerations.

---

# Sprint 13 Deliverables

## Phase 1 — Base MVP

* [x] Project selected: EduCore
* [ ] Create public GitHub repository
* [ ] Repository name: `prodesk-capstone-educore`
* [ ] Create comprehensive README / PRD
* [ ] Define project name
* [ ] Define designated track
* [ ] Define technology stack
* [ ] Define prioritized core features

## Phase 2 — Priority 1

* [ ] Create Figma project
* [ ] Design minimum three core screens
* [ ] Add public Figma link to README

## Phase 3 — Priority 2 / Stretch

* [ ] Create MongoDB ERD
* [ ] Create Redux state tree diagram
* [ ] Define mock API endpoints
* [ ] Export architecture diagram
* [ ] Embed architecture diagram in README

---

# Success Criteria

EduCore's planning phase will be considered successful when the PRD, UI/UX designs, database architecture, Redux state structure, and API plan provide a clear blueprint for implementing the application.

The goal is to establish a scalable and maintainable architecture before beginning development, reducing technical debt and ensuring that the four-week capstone development phase has a clearly defined direction.

---

## Project Status

**Current Phase:** Sprint 13 — Product Planning, System Architecture & UI/UX Design

**Development Status:** Planning and Design

**Next Phase:** Application Development

