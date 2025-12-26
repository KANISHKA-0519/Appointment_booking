# Appointment Booking System

A full-stack appointment booking application with login authentication, built with React.js frontend and Node.js/Express backend with MongoDB.

## Features

- User authentication (Login/Logout)
- Book new appointments
- View all appointments
- Update appointment status (pending, confirmed, cancelled)
- Delete appointments
- Responsive design

## Tech Stack

**Frontend:**
- React.js
- HTML5
- CSS3
- JavaScript (ES6+)

**Backend:**
- Node.js
- Express.js
- MongoDB
- Mongoose

## Complete Setup Instructions

### Prerequisites
- Node.js installed
- MongoDB installed

### Step 1: Install MongoDB
1. Download MongoDB Community Server from https://www.mongodb.com/try/download/community
2. Install with default settings
3. Create data directory: `mkdir C:\data\db`

### Step 2: Start MongoDB
```bash
"C:\Program Files\MongoDB\Server\8.2\bin\mongod.exe" --dbpath C:\data\db
```
Keep this terminal open.

### Step 3: Setup Backend
```bash
cd backend
npm install
npm run dev
```
Backend runs on http://localhost:5000

### Step 4: Setup Frontend
```bash
cd frontend
npm install
npm start
```
Frontend runs on http://localhost:3000

### Step 5: Login
- Username: **admin**
- Password: **admin123**

## API Endpoints

- `GET /api/appointments` - Get all appointments
- `POST /api/appointments` - Create new appointment
- `PATCH /api/appointments/:id` - Update appointment status
- `DELETE /api/appointments/:id` - Delete appointment

## Usage

1. Login with admin/admin123
2. Fill out the booking form with details
3. Select service type and date/time
4. Click "Book Appointment"
5. Manage appointments (confirm/cancel/delete)
6. Logout when done

## Project Structure
```
appointment_booking/
├── backend/
│   ├── models/
│   │   └── Appointment.js
│   ├── package.json
│   ├── server.js
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── App.js
│   │   ├── App.css
│   │   ├── Login.js
│   │   ├── Login.css
│   │   └── index.js
│   └── package.json
└── README.md
```