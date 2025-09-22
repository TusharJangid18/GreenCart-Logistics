# GreenCart Logistics - Full Stack Assessment Project

## Overview
A full-stack application for simulating delivery operations and calculating KPIs for GreenCart Logistics. Built with Node.js/Express (backend), React/TypeScript (frontend), and MongoDB.

## Features
- JWT Authentication
- Dashboard with KPIs and Charts (Recharts)
- Simulation Engine with Company Rules
- CRUD for Drivers, Routes, Orders
- Responsive UI (Tailwind CSS)

## Tech Stack
- Backend: Node.js, Express, Mongoose, JWT, bcrypt
- Frontend: React 18, TypeScript, Axios, React Router, Recharts, Tailwind
- Database: MongoDB Atlas

## Setup
1. Clone repo: `git clone https://github.com/TusharJangid18/GreenCart-Logistics.git`
2. Backend: `cd backend && npm install && npm run dev`
3. Frontend: `cd frontend && npm install && npm start`
4. Database: Update backend .env with MongoDB Atlas URI
5. Login: username=manager, password=pass123

## Deployment
- Backend: Render.com
- Frontend: Vercel
- DB: MongoDB Atlas

## API Endpoints
- POST /api/auth/login
- GET/POST/PUT/DELETE /api/drivers
- Similar for /routes, /orders
- POST /api/simulation/run
- GET /api/simulation/history

## Testing
- Backend: `npm test` (Jest)
- Frontend: `npm test`

## Company Rules Implemented
1. Late Penalty: ₹50 if >10min late
2. Fatigue: >56h/week = 30% slower
3. Bonus: 10% for >₹1000 on-time orders
4. Fuel: ₹5/km base + ₹2/km high traffic
5. Profit: Value + Bonus - Penalties - Fuel
6. Efficiency: (On-time/Total) * 100

Built by Tushar Jangid for Purple Merit Assessment - September 2025
