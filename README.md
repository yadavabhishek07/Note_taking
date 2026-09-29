# Note-Taking App

A secure, minimalist note-sharing web application featuring time-based expiration, one-time self-destruct links, and optional dynamic password protection.

🔗 **Live Demo:** [https://note-taking-app-phi-ten.vercel.app](https://note-taking-app-phi-ten.vercel.app)

---

## Overview

Note-Taking App is a privacy-focused web application that allows users to write notes and share them using expiring links. With built-in support for one-time burning links, password access control, and an owner management dashboard, your sensitive notes stay protected.

---

## Key Features

- **Self-Destructing Notes**: One-time view links that automatically burn and delete permanently after being read.
- **Expiring Links**: Configurable time-based expiration (1 hour, 24 hours, or 7 days).
- **Password Protection**: Optional dynamic passcode protection for shared notes.
- **Owner Dashboard**: View created notes, track link status, and instantly revoke access anytime.
- **Zero-Config Database**: Works immediately out-of-the-box with embedded PGlite (WASM PostgreSQL) or external PostgreSQL.

---

## Tech Stack

- **Frontend**: Next.js 14 (App Router), React, TypeScript, Tailwind CSS
- **Backend API**: Next.js Serverless Route Handlers & Hono.js
- **Database**: PostgreSQL with Drizzle ORM (embedded PGlite support)
- **Authentication**: JWT Session Cookies & bcryptjs
- **Hosting**: Vercel

---

## Local Setup

### 1. Installation
```bash
npm install
```

### 2. Environment Configuration (Optional)
The application works immediately with zero configuration using the embedded database. To connect to an external PostgreSQL database instead, create a `.env` file:
```env
DATABASE_URL="postgresql://user:password@localhost:5432/note_taking_db"
JWT_SECRET="your-secret-key"
```

### 3. Run the App
```bash
# Start development server
npm run dev

# Or build and run for production
npm run build
npm start
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## Author

**Abhishek Yadav**  
GitHub: [@yadavabhishek07](https://github.com/yadavabhishek07)
