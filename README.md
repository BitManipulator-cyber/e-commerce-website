# Vacation Rental Platform

Full-stack web application for listing, searching, and booking vacation rentals, built with the MERN stack (MongoDB, Express.js, React, Node.js) following MVC architecture

## Features

- User authentication and authorization with JWT or similar mechanisms.
- Property listings with images, descriptions, pricing, and availability calendars.
- Search and filter rentals by location, dates, guests, and amenities.
- Booking system with reservation management and payment integration.
- User dashboards for hosts (manage listings) and guests (view bookings).

## Folder structure
> Organized in MVC pattern with clear separation of concerns.

```bash
├── controllers/     # Request handlers (Controllers)
├── models/          # Database schemas (Models)
├── routes/          # API endpoints
├── utils/           # Helper functions
├── views/           # Frontend templates (if server-rendered)
├── app.js           # Main Express app
├── server.js        # Server entry point
├── package.json     # Dependencies
└── config.js        # Configuration
```

## Tech Stack

- MongoDB: NoSQL database for properties, users, and bookings.
- Express.js: Backend framework with MVC routing.
- React: Dynamic frontend UI.
- Node.js: Runtime environment

## Installation steps
> Backend typically runs on http://localhost:5000 and frontend on http://localhost:3000.

```bash
# Clone the repository
git clone https://github.com/BitManipulator-cyber/e-commerce-website.git
cd e-commerce-website

# Install backend dependencies
npm install

# Create .env file for environment variables
cp .env.example .env  # or manually create

# Set up MongoDB connection in .env:
# MONGO_URI=mongodb://localhost:27017/vacation-rentals
# JWT_SECRET=your_super_secret_key_here
# PORT=5000

# Start MongoDB service (if local)
mongosh  # or use MongoDB Atlas URI

# Run backend development server
npm run dev  # Uses nodemon for auto-restart

# In a new terminal, for frontend (if separate client folder exists):
cd client
npm install
npm start  # Runs on http://localhost:3000
```
