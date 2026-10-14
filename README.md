# CacheUp — Next-Gen Learning Management System (LMS)

A functional, responsive, and aesthetically modern **Learning Management System (LMS)** crafted with **React.js**, **Vite**, and **Tailwind CSS v4**, styled after the **ART ACADEMY** and **Learnthru** design inspirations with the official **CacheUp visual identity guidelines**.

Ready for direct upload to **GitHub** and instant one-click deployment to **Vercel**.

---

## 🎨 Visual Identity & Brand System

CacheUp implements the strict design specifications from the visual identity guidelines:

### Color Palette
- **Forest (`#1E3F33`)**: Primary brand color for headings, primary buttons, accents, and navigation pills.
- **Sage (`#9CB49A`)**: Soft organic tone for secondary badges, subtle borders, card highlights, and progress states.
- **Cream (`#FAF7EF`)**: Warm, premium ivory canvas background and soft card containers.
- **White (`#FFFFFF`)**: Crisp, elevated card surfaces with subtle micro-shadows.
- **Charcoal (`#232724`)**: High-contrast dark cards, deep typography, and selected states.
- **Gold (`#DE9E36`)**: Radiant warm gold for active navigation items, achievement honors, and high-priority indicators.

### Typography
- **Headings**: `Plus Jakarta Sans` (page titles, section headings, course titles, greetings)
- **Body**: `DM Sans` (paragraphs, navigation links, buttons, form labels, assignment details, tables)

---

## 📱 UI/UX Layout Architecture

Replicating the multi-column layout from the inspiration previews:

1. **Left Navigation Sidebar**:
   - CacheUp geometric emblem & brand identity
   - Dynamic navigation items tailored to the active role
   - Live badge counters (pending submissions, unread announcements, due tasks)
   - Dark **Help Center** promo card with quick ticket modal
   - Secure sign-out action

2. **Center Main Workspace**:
   - Header with friendly greeting (`Hello Stella 👋`, `Let's learn something new today!`)
   - Global interactive search bar
   - One-click **Instant Demo Role Switcher** (`Student` | `Teacher` | `Admin`)
   - Reset Demo Data button
   - Notification bell with unread dropdown popover
   - Dynamic page view router for all 21 system pages

3. **Right Profile & Schedule Panel**:
   - Profile card with avatar, role, and quick jump to profile
   - **Interactive Calendar**: month navigation (`<` / `>`), active day highlighting, dots on class dates
   - **Daily Schedule**: color-coded time-blocked session cards (*Sketching 12:00*, *History of Art 14:30*)
   - **Reminders**: upcoming deadlines and quiz notices
   - Collapsible on desktop / responsive drawer on mobile

---

## 🚀 All 21 Pages Implemented

CacheUp includes complete, functional implementations for all 21 specified pages:

1. **Login**: User authentication with email/password and one-click demo presets.
2. **Student Registration**: Prospective students register with department, bio, and portfolio link.
3. **Registration Pending / Approval**: Admin reviews applicants, verifies credentials, and approves or rejects accounts.
4. **Student Dashboard**: Progress overview, enrolled course cards with progress bars, assignments, and home task cards.
5. **Teacher Dashboard**: Teacher responsibilities, courses managed, and submission grading queues.
6. **Admin Dashboard**: Platform-wide metrics (students, faculty, courses, pending approvals) and infrastructure health.
7. **User Management**: Admin can search, filter, promote roles (Student/Teacher/Admin), and delete accounts.
8. **Browse / My Courses**: Course directory with category pills (*Fine Arts, Illustration, Typography, CS*), search, and enrollment toggles.
9. **Course Details**: Full course syllabus, lesson breakdown, enrolled classmates directory, and attached resources.
10. **Create / Edit Course**: Form to author course metadata, schedule, room, cover image, and syllabus units.
11. **Learning Materials**: Resource repository with file-type filters (PDF, Slides, Video, Code, Image), download simulation, and teacher upload portal.
12. **Assignment Details**: Task instructions, due dates, maximum points, rubrics breakdown, and submission CTA.
13. **Create / Edit Assignment**: Teachers author tasks with custom rubrics and priority tags.
14. **Assignment Submission**: Students submit answers, repository URLs, simulate file uploads, and receive celebratory confetti.
15. **Submission Review**: Teachers inspect student submissions filtered by course and status.
16. **Grading & Feedback**: Interactive grading modal with score input, automatic letter grade calculation, and qualitative feedback.
17. **My Grades**: Complete gradebook with GPA calculation, letter grades, percentage scores, and teacher critique notes.
18. **My Progress**: Track completion analytics, study hours, streak counter, honors badges, and printable PDF transcript.
19. **Announcements / Notifications**: Teachers and admins publish campus bulletins with priority tags; users view and mark as read.
20. **Profile**: User profile view with avatar, student ID, department, contact info, and course history.
21. **Account Settings**: Profile updates, password changes, and notification preference toggles.

---

## ⚡ Instant Demo Credentials

Use the **One-Click Demo Switcher** in the header or sign in with:

| Role | Name | Email | Password |
|---|---|---|---|
| **Student** | Stella Walton | `stella@cacheup.edu` | `password123` |
| **Student** | Melissa Anderson | `melissa@cacheup.edu` | `password123` |
| **Teacher** | Prof. Alicia Mayer | `alicia@cacheup.edu` | `password123` |
| **Teacher** | Mika Dickens | `mika@cacheup.edu` | `password123` |
| **Admin** | Marcus Vance | `admin@cacheup.edu` | `password123` |

*Prospective Student awaiting approval*: `Lucas Perez` (`lucas.perez@example.com`).

---

## 🛠️ Local Development

```bash
# 1. Install dependencies
npm install

# 2. Start local development server
npm run dev

# 3. Test production build
npm run build
```

---

## 🌐 Deploy to GitHub & Vercel

### Step 1: Initialize Git and Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit: CacheUp Learning Management System"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```

### Step 2: Deploy to Vercel
1. Log in to [Vercel](https://vercel.com)
2. Click **"Add New Project"** and select your GitHub repository
3. Framework Preset will automatically detect **Vite**
4. Root Directory: `./`
5. Click **"Deploy"**!

The pre-configured `vercel.json` ensures that all routes and client-side page state resolve cleanly with zero 404 errors.
