# EduCore

## Enterprise Learning Management System

EduCore is an Enterprise Learning Management System designed to bring students, instructors, and administrators together on one platform. The system will make it easier for students to access courses and track their learning, while instructors can manage educational content and student activities.

This project is being developed as part of the Prodesk IT Capstone Phase.

---

## Project Information

| Field | Details |
|---|---|
| Project Name | EduCore |
| Project Type | Enterprise Learning Management System (LMS) |
| Designated Track | Full Stack Web Development |
| Project Phase | Capstone Phase |
| Development Duration | 4 Weeks |
| Repository | `prodesk-capstone-educore` |

---

# Project Objective

The main objective of EduCore is to create a centralized learning platform where students can manage their courses and academic activities, instructors can manage learning content and evaluate students, and administrators can manage the overall platform.

The application will focus on providing a clean dashboard-based experience with role-specific features.

---

# Target Users

EduCore will have three main types of users.

### 1. Student

Students will use EduCore to:

- Browse and enroll in courses
- Access course lessons
- Track their learning progress
- View assignments
- Submit assignments
- Attempt quizzes
- View grades and results
- Receive important notifications

### 2. Instructor

Instructors will use EduCore to:

- Create and manage courses
- Add and manage lessons
- Create assignments and quizzes
- View student submissions
- Grade assignments
- View enrolled students
- Monitor student performance

### 3. Administrator

Administrators will manage the overall platform and will be able to:

- Manage users
- Manage students and instructors
- Manage courses
- Monitor platform activity
- View basic platform statistics

---

# Technology Stack

The project will use the following technologies:

### Frontend

- React
- JavaScript
- Vite
- Redux Toolkit
- CSS

### Backend

- Node.js
- Express.js

### Database

- MongoDB

### API

- REST API

### Authentication

- JWT-based authentication

### Design and Planning

- Figma for UI/UX design
- Draw.io for system architecture diagrams

### Version Control

- Git
- GitHub

### Deployment

- Vercel for frontend deployment
- MongoDB Atlas for cloud database
- Backend hosting will be finalized during development

---

# Core Features

The features are divided into three priority levels so that the most important functionality is completed first.

## P0 — Mandatory Core Features

These features make up the Base MVP and are the main focus of the project.

### Authentication and Authorization

- User registration
- User login and logout
- Protected pages
- Role-based access for Students, Instructors, and Administrators

### Student Dashboard

Students will have a dashboard showing:

- Enrolled courses
- Learning progress
- Upcoming assignments
- Recent grades
- Notifications

### Course Management

Students can:

- Browse available courses
- View course details
- Enroll in courses
- Access enrolled courses

Instructors can:

- Create courses
- Edit courses
- Delete courses
- Add and manage lessons

Administrators can manage courses across the platform.

### Lessons and Progress

Students can:

- View course lessons
- Mark lessons as completed
- Track their course completion progress
- Continue learning from their previous progress

### Assignments

Students can:

- View assignments
- See assignment instructions
- Check deadlines
- Submit assignments
- View their grades

Instructors can:

- Create assignments
- Set deadlines
- View student submissions
- Grade submissions

### Quizzes

Students can:

- Attempt quizzes
- Submit answers
- View quiz results

Instructors can:

- Create quizzes
- Add questions and options
- Set correct answers
- View student results

### Grades

Students can view:

- Assignment grades
- Quiz results
- Overall course performance

Instructors can review and manage student performance.

### Basic User Management

Administrators can:

- View users
- Manage student and instructor accounts
- Activate or deactivate accounts

---

# P1 — Priority Features

After the Base MVP is completed, the following features will be considered:

- Course search
- Course filtering
- Notifications
- Calendar
- Student performance analytics
- Instructor analytics
- Improved administrator dashboard
- Course progress reports

These features will be implemented depending on the progress of the MVP.

---

# P2 — Stretch Features

The following features are optional and will only be considered after the main application is stable:

- AI learning assistant
- AI-based course recommendations
- Personalized learning suggestions
- Advanced analytics
- Real-time notifications

These features are not required for the Base MVP.

---

# Main Application Views

The initial UI/UX design will focus on the following screens:

1. Authentication / Login
2. Student Dashboard
3. Course Details
4. Instructor Dashboard
5. Assignment Details
6. Admin Dashboard

The first three screens will satisfy the minimum UI/UX design requirement, while the remaining screens will be developed as additional designs.

---

# Planned Application Flow

The basic user flow will be:

```text
User
  ↓
Login / Registration
  ↓
Role Verification
  ↓
Role-specific Dashboard
  ↓
Courses / Assignments / Quizzes
  ↓
Progress and Results

## Figma Design

The UI/UX wireframes for EduCore were designed in Figma.

### Core Viewports

1. Authentication Screen
2. Student Dashboard
3. Course Details View

**Figma Design:** [View EduCore UI/UX Design](https://www.figma.com/design/4YCqEvMVBHqrlVomCSmoYh/EduCore-%E2%80%94-UI-UX-Design?node-id=0-1&t=HBuaAd0saUzrIWPO-1)
