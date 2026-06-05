# Learner's Guide Platform

A production-ready Learner's Guide platform built with React, Vite, Tailwind CSS, React Router, and Supabase.

## Project structure

- `src/`
  - `components/` — shared UI helpers and route guards.
  - `pages/` — landing, login, signup, student, teacher, parent, admin, and 404 pages.
  - `contexts/` — authentication context and session handling.
  - `services/` — Supabase access and local fallback data layer.
  - `assets/` — assets and images.
  - `App.jsx` — root React app.
  - `main.jsx` — Vite bootstrap.
  - `router.jsx` — app route definitions.
- `supabase/schema.sql` — Supabase-compatible schema.
- `.github/workflows/deploy.yml` — GitHub Actions build workflow.
- `.env.example` — template environment variables.

## Setup

1. Copy `.env.example` to `.env`.
2. Set `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY`.
3. Install dependencies:

```bash
npm install
```

4. Start the development server:

```bash
npm run dev
```

## Supabase configuration

Add these values to `.env`:

```env
VITE_SUPABASE_URL=https://YOUR_SUPABASE_PROJECT.supabase.co
VITE_SUPABASE_ANON_KEY=YOUR_SUPABASE_ANON_KEY
```

The app uses `src/services/supabase.js` for centralized Supabase client access and `src/services/db.js` for authenticated REST queries and local fallback behavior.

## Deploy on Vercel

1. Push the repository to GitHub.
2. Connect the project in Vercel.
3. Add the same environment variables in Vercel.
4. Set the build command to `npm run build` and output directory to `dist`.

## Legacy code

The originally uploaded files are preserved in `src/legacy/`.
