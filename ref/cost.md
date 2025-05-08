# 💰 MGM Institute – Project Cost Breakdown

This document outlines the estimated development costs for MGM Institute based on task segmentation (UI, APIs, database, labor, and branding).

---

## 📱 UI/UX Development Cost

**Rate:** `$5 per page/screen`

| UI Section         | Pages / Screens | Cost  |
|--------------------|------------------|-------|
| Landing Page       | 1                | $5    |
| Sign In / Sign Up  | 2                | $10   |
| Course Listing     | 1                | $5    |
| Course Overview    | 1                | $5    |
| Student Dashboard  | 5 (Grades, Courses, Coursework, Notifications, Inbox) | $25 |
| Instructor Dashboard | 6 (Courses, Gradebook, Notifications, Profile, Inbox, Payments) | $30 |
| Admin Panel        | 5 (Users, Grades, Courses, Events, Payments) | $25   |
| Profile Management | 1 each for all roles | $5 x 3 = $15 |
| Course Creation (Multi-step form) | 3 screens | $15 |
| Forums/Discussions | 1                | $5    |
| Misc (Settings, 404, Terms) | 3     | $15   |

**🎯 Total UI Cost:** `$155`

---

## 🔗 Backend API Development Cost

**Rate:** `$10 per API`

Includes: route logic, DB connection, validation, authentication, authorization, and security patches.

### 🔐 Authentication & User Management APIs

| API Function        | Endpoint Example            | Cost |
|---------------------|-----------------------------|------|
| Register User       | `POST /api/auth/register`   | $10  |
| Login User          | `POST /api/auth/login`      | $10  |
| Edit Profile        | `PUT /api/users/:id`        | $10  |
| Fetch User Profile  | `GET /api/users/:id`        | $10  |

**Subtotal:** `$40`

---

### 🎓 Student APIs

| API Function                      | Endpoint Example                  | Cost |
|-----------------------------------|-----------------------------------|------|
| Purchase Course                   | `POST /api/courses/:id/purchase`  | $10  |
| View Enrolled Courses             | `GET /api/students/:id/courses`   | $10  |
| Get Grades                        | `GET /api/students/:id/grades`    | $10  |
| Coursework                        | `GET /api/students/:id/coursework`| $10  |
| Notifications                    | `GET /api/students/:id/notifications` | $10  |
| Inbox                            | `GET /api/students/:id/messages`  | $10  |

**Subtotal:** `$60`

---

### 👨‍🏫 Instructor APIs

| API Function                     | Endpoint Example                    | Cost |
|----------------------------------|-------------------------------------|------|
| Create Course                    | `POST /api/instructors/:id/courses` | $10  |
| Add Chapter / Subchapter        | `POST /api/courses/:id/chapters`    | $10  |
| Add Assignment / Quiz / Exam    | `POST /api/chapters/:id/assessments`| $10  |
| View All Courses                | `GET /api/instructors/:id/courses`  | $10  |
| View Grades                     | `GET /api/courses/:id/grades`       | $10  |
| Notifications                   | `POST /api/instructors/:id/notify`  | $10  |
| Payment Logs                    | `GET /api/instructors/:id/payments` | $10  |
| Inbox                           | `GET /api/instructors/:id/messages` | $10  |

**Subtotal:** `$80`

---

### 🛡 Admin APIs

| API Function                   | Endpoint Example                     | Cost |
|--------------------------------|--------------------------------------|------|
| View All Grades                | `GET /api/admin/grades`              | $10  |
| View All Students              | `GET /api/admin/students`            | $10  |
| View All Payments              | `GET /api/admin/payments`            | $10  |
| Manage Suspensions             | `PATCH /api/admin/suspend`           | $10  |
| Post Notification              | `POST /api/admin/notifications`      | $10  |
| Schedule Events                | `POST /api/admin/events`             | $10  |

**Subtotal:** `$60`

---

### 📂 Course Overview & Public APIs

| API Function                   | Endpoint Example                    | Cost |
|--------------------------------|-------------------------------------|------|
| Get Categories                 | `GET /api/categories`               | $10  |
| Get Courses by Category        | `GET /api/categories/:id/courses`   | $10  |
| Course Overview                | `GET /api/courses/:id`              | $10  |

**Subtotal:** `$30`

---

### 📊 Total Backend API Cost: **`$270`**

---

## 🗃 Database Setup & Management

| Task                          | Description                                               | Cost |
|-------------------------------|-----------------------------------------------------------|------|
| Schema Design (Users, Courses, Grades, etc.) | Entity relationship design + migrations | $30  |
| Data Seeding (dummy data)     | Insert base users, test data for demo                    | $10  |
| Backup & Monitoring Setup     | Cron or admin backup tools                               | $10  |

**Total Database Cost:** `$50`

---

## 🔐 Security & Server Handling

| Feature                      | Description                                                   | Cost |
|-----------------------------|---------------------------------------------------------------|------|
| Rate Limiting               | Protect endpoints (e.g., login, sensitive ops)                | $10  |
| Token-Based Auth Setup      | JWT / Session cookie for auth                                 | $10  |
| Role-based Access Control   | Middleware + DB model for admin/instructor/student separation | $10  |
| API Request Monitoring Logs | Custom logging for suspicious API hits                        | $10  |

**Total Security Cost:** `$40`

---

## 🎨 Branding & Labor

| Task            | Description                     | Cost  |
|-----------------|----------------------------------|-------|
| Logo Design     | Unique brand identity logo       | $100  |
| Icon Set        | Custom icon design (Favicon etc) | $100  |
| General Labor   | Communication, QA, deployment    | $500  |

---

## ✅ Final Cost Summary

| Component              | Cost  |
|------------------------|-------|
| UI/UX Pages            | $155  |
| Backend APIs           | $270  |
| Database Setup         | $50   |
| Security & Access Ctrl | $40   |
| Logo Design            | $100  |
| Icon Design            | $100  |
| General Labor          | $500  |

### 💵 **Total Estimated Project Cost: `$1,215`**

---

> ⚠️ These are development-time estimates and do not include server hosting, domain, or third-party integrations (e.g., email, video storage).
