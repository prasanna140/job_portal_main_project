# 🌸 BloomJobs

A modern, responsive job portal front end — browse and search listings, view
job details, submit multi-step applications, save jobs, and manage your
account from a personal dashboard and profile page.

This is a **client-only** demo: there's no backend. Accounts and application
data are stored in the browser's `localStorage`, which is enough to make the
whole flow (sign up → browse → apply → track in dashboard) actually work,
but it is **not** a substitute for real authentication or a database — don't
reuse the auth pattern here for anything handling real user data.

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6 Modules)
- LocalStorage API
- JSON (jobs.json)
- Responsive Web Design

## Features

- Email/password sign up with live password-strength feedback, and sign in
- Searchable, filterable job listings (type, location, category, quick tags)
- Detailed job pages with save/apply actions
- A 3-step application modal (personal info → experience/resume/skills →
  cover letter) with inline validation, drag-and-drop resume upload, and a
  skill-chip picker
- A dashboard summarizing applied/saved jobs
- A profile page to edit your display name, bio and avatar
- Toast notifications and a confirm-before-sign-out dialog
- Fully responsive layout down to small phone widths



### Architecture notes

- The application is organized using modular JavaScript (ES6 Modules).
- `app.js` acts as the main entry point and initializes the application.
- Feature-specific logic is separated into dedicated modules such as authentication, job management, dashboard, and profile.
- Shared utility functions and reusable components are organized into separate files to improve maintainability.
- Application data is persisted using the browser's LocalStorage API.
- The modular architecture makes the project easier to maintain, extend, and debug.

## Known limitations (by design, since this is a demo)

- Passwords are stored in plain text in `localStorage` — fine for a local
  demo, not for production.
- There's no server-side validation, rate limiting, or duplicate-email
  protection beyond what the client checks.
- Data lives in one browser's `localStorage`, so accounts won't sync across
  devices or browsers.

## Screenshots
![image alt](https://github.com/prasanna140/job_portal_main_project/blob/41676ae49f7e4ea596eb2f920ccbde9ff3aa12b6/job_portal_showcases.png)

## Future Improvements

- Backend integration with Node.js and MongoDB
- Email verification
- Forgot Password functionality
- Company Dashboard
- Admin Panel
- Real-time job notifications
- Resume Builder
- AI-powered Job Recommendations
- Interview Scheduling
- Dark Mode
