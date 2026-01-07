# AI Study Companion (Phase 1)

A full-stack groundwork for an AI study companion app.

## Project Structure

- `client/`: Next.js frontend (JavaScript, App Router)
- `server/`: Express + Node.js backend
  - `src/`: Source code
  - `prisma/`: Database schema

## Prerequisites

- Node.js
- MySQL Database running locally or in cloud
- npm

## Setup & Run

### 1. Database Setup
Create a MySQL database (e.g., `study_companion`) and update `server/.env` with your credentials:
```env
DATABASE_URL="mysql://USER:PASSWORD@HOST:PORT/DATABASE"
```

Then run migrations:
```bash
cd server
npx prisma migrate dev --name init
```

### 2. Backend
```bash
cd server
npm install
npm run dev
```
Server runs on `http://localhost:4000`.
Health check: `http://localhost:4000/`

### 3. Frontend
```bash
cd client
npm install
npm run dev
```
Frontend runs on `http://localhost:3000`.

## Features (Phase 1)
- Express API framework
- Prisma ORM with MySQL
- Models: User, Document, Chat
- Next.js 14+ Frontend scaffolding
# ai-companion
