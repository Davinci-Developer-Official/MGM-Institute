# 🎓 MGM Institute – Project Overview

MGM Institute is an online learning platform focused on **gender studies** and **women empowerment**. It provides structured learning through instructor-led courses, interactive content, assessments, and community engagement.

---

## 🧩 Key Features

### 🏠 Public Landing Page
- Overview of MGM’s mission and values
- Course categories and featured courses
- Information about institution leadership
- Sign-in and sign-up options

---

## 👤 User Roles

### 1. **Student**
- Browse & purchase courses
- View enrolled courses and course materials
- Track grades:
  - Filterable by course, assignments, quizzes, and exams
- Coursework section (same filters as grades)
- Real-time notifications:
  - From admin, instructors, or course alerts
- Inbox for direct messaging
- Manage profile and settings

---

### 2. **Instructor**
- Create and manage courses
- Upload:
  - Chapters, sub-chapters
  - Assignments (per chapter)
  - Quizzes (per sub-chapter)
  - Final exams (per course)
- View all their courses (active/closed)
- Grade student submissions
- View class performance and individual student grades
- Notifications (limited to own courses)
- View payment logs (filterable)
- Manage own profile and messaging inbox

---

### 3. **Admin**
- Post platform-wide notifications
- Create & schedule events
- View all students and their records (biodata, academic)
- Monitor grades across all courses (filterable)
- Manage all payments (commission tracking per course)
- Suspend students, instructors, courses, or payments
- Full access to the system for oversight and security

---

## 📝 Course Structure

Each course consists of:
- Main chapters and sub-chapters
- Assignments (chapter-based)
- Quizzes (subchapter-based)
- Final exam
- Discussion forum for questions and answers

All assessments contribute to the **final grade**.

---

## 🔗 System Architecture (Overview)

- Frontend: Built with **Next.js** using **TypeScript** and **Tailwind CSS**
- Backend: RESTful API architecture (Node.js or Next.js API routes)
- Database: PostgreSQL with role-based access
- Authentication: JWT or session-based
- File Storage: For assignments and exams (e.g., Vercel Blob or AWS S3)
- Notifications: Real-time via WebSocket or polling
- Messaging: Internal inbox system between roles
- Payment: Integrated with course purchase tracking and instructor payouts

---

## 🔐 Access Privileges

| Feature               | Student | Instructor | Admin  |
|-----------------------|---------|------------|--------|
| View/Purchase Courses | ✅      | ❌         | ❌     |
| Create Courses        | ❌      | ✅         | ❌     |
| Grade Students        | ❌      | ✅         | ✅     |
| View All Grades       | ❌      | ❌         | ✅     |
| Post Notifications    | ❌      | ✅ (limited)| ✅     |
| Suspend Actions       | ❌      | ❌         | ✅     |
| Inbox Messaging       | ✅      | ✅         | ✅     |

---

## 🚀 Development Status

This overview serves as a reference during project development. Each section is independently managed but interconnected for seamless operation.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
