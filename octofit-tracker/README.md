# 🐙 OctoFit Tracker

A modern multi-tier fitness tracking application built with React 19, Node.js/Express, and MongoDB.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
├── backend/           # Node.js + Express + TypeScript API
└── README.md          # This file
```

## Technology Stack

### Frontend
- **React 19** - UI library
- **Vite** - Build tool and dev server
- **TypeScript** - Type safety
- **Port:** 5173

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **TypeScript** - Type safety
- **Mongoose** - MongoDB object modeling
- **Port:** 8000

### Database
- **MongoDB** - NoSQL database
- **Port:** 27017

## Getting Started

### Prerequisites
- Node.js 18+ and npm
- MongoDB installed and running locally OR Docker

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install

# Create .env file from example
cp .env.example .env

# Start development server
npm run dev
```

The backend API will be available at `http://localhost:8000`

### MongoDB Setup

If using Docker:

```bash
docker run -d -p 27017:27017 --name octofit-mongo mongo:latest
```

Or install MongoDB locally and ensure it's running on port 27017.

## Available Scripts

### Frontend

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Backend

- `npm run dev` - Start development server with ts-node
- `npm run build` - Compile TypeScript to JavaScript
- `npm run start` - Run compiled JavaScript
- `npm run lint` - Run ESLint

## API Endpoints

- `GET /` - API info
- `GET /health` - Health check
- `GET /api/*` - API routes (to be implemented)

## Port Configuration

| Service    | Port  |
|-----------|-------|
| Frontend  | 5173  |
| Backend   | 8000  |
| MongoDB   | 27017 |

## Development

The frontend Vite config includes a proxy to the backend, so API calls to `/api/*` will be forwarded to `http://localhost:8000/*`.

## Next Steps

1. ✅ Initialize project structure
2. ⏳ Create database models (User, Workout, etc.)
3. ⏳ Build API endpoints
4. ⏳ Implement authentication
5. ⏳ Build React components
6. ⏳ Add state management
7. ⏳ Deploy to production

## License

MIT
