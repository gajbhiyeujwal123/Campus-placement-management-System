# CampusCare — Premium TKIET Frontend

Responsive React + TypeScript + Tailwind CSS v4 concept for the Campus Complaint Management System.

## Run
Requires Node.js 20+.
```bash
npm install
npm run dev
```
Production build:
```bash
npm run build
npm run preview
```

## Included screens
- Overview dashboard
- My complaints (search, status filters, CSV export)
- Submit a complaint (client-side validation, in-memory demo creation)
- Analytics (area, donut, composed bar/line, horizontal bar, radar)
- Departments
- Help centre

## Design
Dark-first with working light/dark toggle, deep ink surfaces, restrained violet and mint accents, responsive sidebar, CSS-built spatial campus illustration, subtle motion, and reduced-motion support.

## Important limitations
This is a frontend demo, not a production-connected system. Dashboard statistics and chart data are illustrative and not official TKIET data. Complaint data resets on refresh; file selection is local only. Authentication, server-side role enforcement, notifications, audit logs, PostgreSQL persistence, and C++20/Drogon APIs are not connected. Confirm official departments, routing, SLAs, anonymous reporting rules, contacts, and data-retention policy before production.


## Login and intro animation

The app opens with a short animated CampusCare brand intro, followed by the student sign-in screen. The sign-in form is currently a frontend demo only: it validates the email/password fields and opens the dashboard, but it does not authenticate against a server. Connect it to the approved C++ API and identity provider before production use.


## Visual theme
The intro, login screen, and dashboard share a charcoal/near-black foundation with warm orange-copper accents and restrained mint highlights. The dashboard light theme uses a warm off-white background with the same accent palette.

## Profile and notifications

- **Profile** is available from the sidebar and account menu. It includes editable display name, email, phone, programme/department and academic year fields (student role), plus role and security context.
- **Notifications** includes a notification centre, unread/read states, mark-all-as-read, complaint links, and toggles for status, campus announcement and email preferences.
- These account changes and notifications are front-end demo state only. Connect an authenticated backend/database and a notification delivery service before using real student/staff records.
