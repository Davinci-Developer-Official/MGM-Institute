## 📁 Project Structure – MGM Institute (Next.js + TypeScript)

### Root Directory
- `/public`
  - `/assets`
    - `/icons` - SVGs, logos, and other icon files
    - `/images` - Public static images
  - `favicon.ico` - Site favicon

- `/src`
  - `/app`
    - `layout.tsx` - Main application layout
    - `page.tsx` - Landing page

    - `/auth`
      - `/login` - Login page
      - `/register` - Registration page

    - `/student`
      - `/dashboard` - Student homepage
      - `/courses`
        - `/[courseId]`
          - `overview.tsx` - Course overview
          - `/chapters`
            - `/[chapterId]`
              - `/subchapters`
                - `/[subChapterId]` - Subchapter content
      - `/grades` - View grades
      - `/coursework` - Assignments, quizzes, exams
      - `/profile` - Student profile
      - `/notifications` - Real-time alerts
      - `/inbox` - Messaging system

    - `/instructor`
      - `/dashboard` - Instructor homepage
      - `/courses`
        - `/[courseId]` - Course details and management
      - `/grades` - View and manage grades
      - `/notifications` - Compose and receive alerts
      - `/payments` - Payment history and analytics
      - `/profile` - Instructor profile
      - `/inbox` - Messaging system

    - `/admin`
      - `/dashboard` - Admin overview
      - `/grades` - View grades across platform
      - `/students` - Manage student profiles
      - `/payments` - Financial records and commissions
      - `/manage` - Suspend users, courses, payments
      - `/notifications` - Platform-wide alerts and events

    - `/about` - About MGM Institute
    - `/contact` - Contact page

  - `/components`
    - `/layout` - Header, footer, nav, etc.
    - `/forms` - Shared form components
    - `/dashboard` - Dash UI elements
    - `/course` - Course UI components
    - `/ui` - Buttons, modals, cards, etc.

  - `/lib`
    - `/utils` - Helpers, formatters
    - `/api` - Axios configs, fetchers

  - `/middleware`
    - `auth.ts` - Authentication guard
    - `roleCheck.ts` - Role-based access control

  - `/hooks` - Custom React hooks
  - `/context` - Global state/context providers
  - `/styles` - Tailwind & custom CSS
  - `/types` - TypeScript interfaces & types
  - `/constants` - Static values like role enums, config

- `/prisma`
  - `schema.prisma` - Prisma ORM schema

- `.env` - Environment variables
- `next.config.js` - Next.js config
- `tsconfig.json` - TypeScript config
- `package.json` - Scripts & dependencies
