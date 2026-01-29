# Live Bidding Platform

**Real-time auction platform with WebSocket bidding, race condition prevention, and server-synchronized timers.**

This is my submission for the Live Bidding Platform technical assessment.

---

## Repository Links

**Main Repository:** [live_bidding_main](https://github.com/YOUR_USERNAME/live_bidding_main)

**Individual Components:**

1. **Backend:** [live_bidding_backend](https://github.com/YOUR_USERNAME/live_bidding_backend)
2. **Frontend:** [live_bidding_frontend](https://github.com/YOUR_USERNAME/live_bidding_frontend)

---

## Live Demo

- **Frontend:** [https://your-app.vercel.app](https://your-app.vercel.app)
- **Backend API:** [https://your-api.onrender.com](https://your-api.onrender.com)

---

## Features Implemented

### Core Requirements

- **REST API:** `GET /items` returns auction items with current bid and end time
- **Real-Time Bidding:** Socket.io for instant bid updates across all clients
- **Race Condition Prevention:** Lock mechanism ensures only one bid per item processes at a time
- **Server Time Sync:** Countdown timers synced to server time (prevents client-side manipulation)
- **Visual Feedback:**
  - Green flash animation on bid updates
  - "WINNING" badge when you're the highest bidder
  - "OUTBID" badge when someone outbids you
- **Auction Expiration:** Automatically rejects bids after auction ends
- **Docker Support:** Full containerization with Docker Compose

### Additional Features

- Username registration and tracking
- Display last bidder name
- Modular backend architecture (routes, socket handlers, data models)
- Environment variable configuration
- Production-optimized Docker images
- Health checks and restart policies

---

## Architecture

### Tech Stack

**Backend:**

- Node.js + Express (REST API)
- Socket.io (WebSocket real-time communication)
- In-memory data store (extensible to database)

**Frontend:**

- React 18
- Vite (build tool)
- Socket.io-client
- Inline styles (production-ready)

**Infrastructure:**

- Docker + Docker Compose
- Multi-stage builds for optimized images

---

## 📁 Project Structure
