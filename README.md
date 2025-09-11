# Lab Authentication API

Simple Auth API (Express + MySQL + JWT + bcrypt).

## Setup
1. Clone repo: `git clone https://github.com/<username>/lab-auth-api.git`
2. Install: `npm install`
3. Copy env: `cp .env.example .env` and fill values (DB creds, JWT_SECRET)
4. Start: `npm run dev`

## Database (create in MySQL)
CREATE DATABASE lab_auth;
(Create `users` and `revoked_tokens` tables — see project SQL/setup screenshots.)

## Endpoints
- `POST /api/auth/signup` — sign up
- `POST /api/auth/login` — login (returns token)
- `POST /api/auth/logout` — logout (protected)
- `GET  /api/profile` — profile (protected)
