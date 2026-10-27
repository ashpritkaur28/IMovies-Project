# iMovies MVP

A React + Vite frontend and Express + MongoDB backend for a movie ticket booking MVP.

## Requirements
- Node.js 18+
- MongoDB running locally or a MongoDB Atlas URI

## 1. Start MongoDB
Make sure your local MongoDB service is running. Default URI: `mongodb://127.0.0.1:27017/Imovies`.

## 2. Configure and start the backend
```bash
cd server
npm install
```
Copy `.env.example` to `.env`, then set `JWT_SECRET` to a long random secret. Keep `.env` private.

Seed demo movies and showtimes:
```bash
npm run seed
```
Then start the API:
```bash
npm run dev
```
API health check: http://localhost:8000/api/health

## 3. Start the frontend (new terminal)
```bash
cd client
npm install
npm run dev
```
Open http://localhost:5173

## Included MVP features
- Register/login with bcrypt password hashing and JWT authentication
- Movie browsing and search
- Demo showtimes and seat layout
- Booking creation and booked-seat persistence in MongoDB
- Booking history
- Responsive dark cinema-inspired UI


