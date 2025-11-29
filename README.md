# PeerCollab - Peer Review & Collaboration Platform

## Overview
PeerCollab is a professional, full-stack web application designed for students to collaborate on projects, share work, and receive structured peer feedback. Built with modern technologies, it provides a secure, scalable platform for educational collaboration.

## Features

### Student Side
- User authentication (JWT-based)
- Upload project submissions with descriptions and tags
- View assigned peers' projects
- Provide structured feedback with ratings and comments
- Collaborate through shared comment spaces
- Track submission history

### Teacher/Admin Side
- Create and manage peer-review assignments
- Add/remove students
- Monitor collaboration progress
- View analytics (review completion, ratings, participation)
- Manage all submissions

## Tech Stack

### Frontend
- **React** - UI library
- **TypeScript** - Type safety
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **PostCSS** - CSS processing

### Backend
- **Node.js** - Runtime
- **Express** - Web framework
- **Drizzle ORM** - Database management
- **JWT** - Authentication

### Database
- **PostgreSQL** (recommended) or suitable relational DB

## Project Structure
```
.
├── client/           # React frontend
├── server/           # Express backend
│   ├── routes/       # API routes
│   ├── controllers/  # Business logic
│   └── models/       # Database models
├── shared/           # Shared utilities
├── script/           # Utility scripts
├── package.json      # Dependencies
└── tsconfig.json     # TypeScript config
```

## Installation

### Prerequisites
- Node.js v16+
- npm or yarn

### Setup

1. Clone the repository
2. Install dependencies: `npm install`
3. Configure environment variables
4. Run database migrations
5. Start development server: `npm run dev`

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login
- `POST /api/auth/logout` - Logout

### Submissions
- `POST /api/submissions` - Create submission
- `GET /api/submissions` - Get submissions
- `GET /api/submissions/:id` - Get single submission

### Reviews
- `POST /api/reviews` - Submit review
- `GET /api/reviews` - Get reviews

## Running

Development: `npm run dev:client` & `npm run dev:server`
Production: `npm run build && npm start`

## Contributing
Submit issues and pull requests for improvements

## License
MIT

## Author
Developed as an educational platform for peer collaboration and feedback
