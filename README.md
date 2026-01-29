# Live Bidding Platform

Real-time auction platform with WebSocket bidding, race condition prevention, and server-synchronized timers.

## Repositories

- Backend: [live_bidding_backend](https://github.com/jainendra001/live_bidding_backend)
- Frontend: [live_bidding_frontend](https://github.com/jainendra001/live_bidding_frontend)

## Live Demo

- Frontend: [Deploy Link](https://live-bidding-frontend-sigma.vercel.app/)
- Backend API: [Deploy Link](https://live-bidding-backend-zl9m.onrender.com)

## Features

- REST API for auction items
- Real-time bidding with Socket.io
- Race condition prevention
- Server-synced countdown timers
- Visual feedback on bid updates
- Username tracking
- Auction expiration validation
- Docker containerization

## Tech Stack

Backend: Node.js, Express, Socket.io  
Frontend: React 18, Vite, Socket.io-client  
Infrastructure: Docker, Docker Compose

## Project Structure
```
live_bidding_backend/
├── data/items.js
├── routes/items.js
├── socket/bidHandler.js
├── auction.js
└── Dockerfile

live_bidding_frontend/
├── src/App.jsx
└── Dockerfile
```
## Quick Start

### Docker

```

git clone https://github.com/jainendra001/live_bidding_backend.git
git clone https://github.com/jainendra001/live_bidding_frontend.git
docker-compose up --build

```

Access at http://localhost:5173

### Local Development

Backend:

```

cd live_bidding_backend
npm install
cp .env.example .env
node auction.js

```

Frontend:

```

cd live_bidding_frontend
npm install
cp .env.example .env
npm run dev

```

## Configuration

Backend .env:

```

PORT=3000
FRONTEND_URL=http://localhost:5173
NODE_ENV=development

```

Frontend .env:

```

VITE_API_URL=http://localhost:3000

```

## Deployment

Backend on Render:

- Build: npm install
- Start: node auction.js
- Set FRONTEND_URL environment variable

Frontend on Vercel:

- Framework: Vite
- Build: npm run build
- Set VITE_API_URL environment variable

## Future Prospects

- Database persistence
- JWT authentication
- Bid history
- Email notifications
- Automated testing
- CI/CD pipeline

## Author

Jainendra Tripathy
GitHub: [@jainendra001](https://github.com/jainendra001)

Submission Date: January 29, 2026
