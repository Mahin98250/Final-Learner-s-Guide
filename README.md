You are a senior full-stack engineer.

Your task is to convert this repository into a production-ready Learner's Guide platform using the uploaded React files already present in the repository.

## Goals

Build a complete React + Vite + Supabase application.

The repository contains:

* learners-guide-withlogo-supabase.jsx
* learners-guide-admin-supabase.jsx

Analyze both files completely and preserve all existing functionality.

## Required Actions

### 1. Project Structure

Create a clean production structure:

src/
├── components/
├── pages/
├── layouts/
├── services/
├── hooks/
├── assets/
├── App.jsx
├── main.jsx
└── router.jsx

Move code into appropriate modules.

---

### 2. Routing

Implement React Router.

Required routes:

/ → Landing page
/login → Login
/student → Student dashboard
/teacher → Teacher dashboard
/parent → Parent dashboard
/admin → Admin dashboard

Protect dashboard routes with authentication.

---

### 3. Supabase

The existing code contains Supabase configuration.

Move all Supabase credentials into:

.env

Use:

VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=

Replace hardcoded values everywhere.

Create:

src/services/supabase.js

for centralized Supabase access.

---

### 4. Database Verification

Inspect all tables referenced in the code and generate a complete SQL schema.

Create:

supabase/schema.sql

Include tables such as:

users
students
teachers
attendance
homework
materials
announcements
fees
marks
messages
notifications
batches
timetable
examschedule

Add sensible indexes and primary keys.

---

### 5. UI Upgrade

Keep all functionality.

Improve:

* responsiveness
* spacing
* typography
* cards
* tables
* forms
* mobile experience

Use:

* Tailwind CSS

Create a modern educational SaaS appearance.

Color palette:

Primary: #5B4FE8
Secondary: #F5A623
Success: #22C55E

---

### 6. Security

Remove all secrets from source code.

Use environment variables.

Check authentication logic.

Add route guards.

Prevent unauthorized dashboard access.

---

### 7. Error Handling

Add:

* loading states
* empty states
* error states
* toast notifications

Avoid blank screens.

---

### 8. Deployment

Configure:

* Vite build
* GitHub Actions workflow
* Vercel deployment compatibility

Create:

.github/workflows/deploy.yml

Ensure successful production builds.

---

### 9. Code Quality

Remove duplicate code.

Remove unused variables.

Fix warnings.

Use reusable components.

Add comments only where necessary.

---

### 10. Final Deliverables

When finished:

1. Commit all changes.
2. Generate README.md.
3. Explain project structure.
4. Explain how to connect Supabase.
5. Explain how to deploy on Vercel.
6. List all files created and modified.
7. Push changes to the current branch.

Do not ask for confirmation.

Inspect the entire repository and complete all tasks automatically.
