# 🔁 Project Flowchart – MGM Institute

```plaintext
                      ┌────────────────────────────┐
                      │        Landing Page        │
                      └────────────┬───────────────┘
                                   │
                  ┌────────────────┼─────────────────┐
        ┌─────────▼────────┐  ┌────▼─────┐  ┌────────▼──────┐
        │    Sign In       │  │ About Us │  │   Course List │
        └────────┬─────────┘  └────┬─────┘  └────────┬──────┘
                 │                │                 │
         ┌───────▼────────┐       │         ┌───────▼────────┐
         │ Select Role:   │       └────────►│ View Course     │
         │ Student/Admin/ │                │ Overview         │
         │ Instructor     │                └──────────────────┘
         └───────┬────────┘
                 │
    ┌────────────▼────────────┐
    │    Authenticated View   │
    └────────┬──────┬─────────┘
             │      │
     ┌───────▼┐  ┌──▼──────────┐
     │Student │  │ Instructor  │
     └────┬───┘  └────┬────────┘
          │          │
     ┌────▼────┐ ┌────▼────────┐
     │ Dashboard│ │ Dashboard  │
     └────┬─────┘ └────┬────────┘
          │           │
   ┌──────▼──────┐ ┌──▼────────────────────┐
   │ Courses     │ │ Courses Created       │
   ├─────────────┤ ├───────────────────────┤
   │ Course View │ │ Create/Edit Courses   │
   │ Purchase    │ │ Add Chapters/Subs     │
   └────┬────────┘ │ Assignments/Quizzes   │
        │          └───────┬───────────────┘
 ┌──────▼─────┐     ┌──────▼────┐
 │ Coursework │     │ Grades    │◄────┐
 │ Assignments│     └────┬──────┘     │
 │ Quizzes    │          │            │
 │ Exams      │   ┌──────▼─────┐      │
 └────┬───────┘   │ View Students│────┘
      │           └─────────────┘
┌─────▼─────────┐   ┌──────────────┐
│ View Grades   │   │ Notifications│
└─────┬─────────┘   └────┬─────────┘
      │                 │
┌─────▼──────────┐ ┌────▼──────────┐
│ Notifications  │ │ Inbox         │
└─────┬──────────┘ └────┬──────────┘
      │                 │
 ┌────▼─────┐      ┌────▼─────┐
 │ Profile  │      │ Payments │
 └──────────┘      └──────────┘

                ┌──────────────────┐
                │      Admin       │
                └────────┬─────────┘
                         │
            ┌────────────▼─────────────┐
            │ View All Courses/Users   │
            │ Manage Suspensions       │
            │ Post Notifications       │
            │ Monitor Grades           │
            │ Payments & Commissions   │
            └──────────────────────────┘
