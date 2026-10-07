<pre>
██╗  ██╗ █████╗  ██████╗██╗  ██╗███████╗██████╗
██║  ██║██╔══██╗██╔════╝██║ ██╔╝██╔════╝██╔══██╗
███████║███████║██║     █████╔╝ █████╗  ██║  ██║
██╔══██║██╔══██║██║     ██╔═██╗ ██╔══╝  ██║  ██║
██║  ██║██║  ██║╚██████╗██║  ██╗███████╗██████╔╝
╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚═════╝
</pre>

<h1 align="center">ResQ — Smart Ambulance Management System</h1>

<p align="center">
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=flat&logo=react" />
  <img src="https://img.shields.io/badge/Node.js-Express-339933?style=flat&logo=node.js" />
  <img src="https://img.shields.io/badge/MongoDB-Mongoose-47A248?style=flat&logo=mongodb" />
  <img src="https://img.shields.io/badge/Socket.io-Realtime-010101?style=flat&logo=socket.io" />
  <img src="https://img.shields.io/badge/SIH-Hackathon-orange?style=flat" />
</p>

---

## 🚑 About

**ResQ** is a real-time ambulance dispatch and tracking platform built for the Smart India Hackathon (SIH). It connects patients, ambulance drivers, hospitals, and administrators on a single unified platform — enabling faster emergency response, live GPS tracking, green corridor signal management, and ER pre-alerts.

---

## ✨ Features

- **Live GPS Tracking** — Real-time ambulance location updates via Socket.io
- **Smart Booking** — Patients request ambulances; drivers accept/reject instantly
- **Green Corridor** — Automated traffic signal prioritization along ambulance routes
- **ER Telemetry** — Live vitals (heart rate, SpO₂, BP, temperature) and ECG streaming to hospital ER
- **Pre-Alert System** — Driver sends arrival alert to hospital before reaching
- **Admin Dashboard** — Monitor active emergencies, manage drivers, ambulances, hospitals & customers
- **Role-based Auth** — Separate portals for Admin, Driver, and Customer
- **Activity Logs & Analytics** — Full audit trail and reporting

---

## 🛠️ Tech Stack

| Layer      | Technology                                      |
|------------|-------------------------------------------------|
| Frontend   | React 19, Vite, React Router, Framer Motion, Three.js, Leaflet, Recharts |
| Backend    | Node.js, Express 5, Socket.io 4                 |
| Database   | MongoDB (Mongoose)                              |
| Auth       | JWT + bcryptjs                                  |
| Realtime   | Socket.io (WebSockets)                          |

---

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18
- MongoDB (local or Atlas)

### 1. Clone the repo

```bash
git clone https://github.com/your-username/HACKATHON-SIH.git
cd HACKATHON-SIH
```

### 2. Setup Backend

```bash
cd backend
cp .env.example .env
# Fill in your MONGO_URI and JWT_SECRET in .env
npm install
npm run dev
```

Backend runs on `http://localhost:5000`

### 3. Setup Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend runs on `http://localhost:5173`

### 4. Seed Admin User

```bash
cd backend
node seedAdmin.js
```

---

## 📁 Project Structure

```
HACKATHON-SIH/
├── backend/
│   ├── controllers/        # Auth & item controllers
│   ├── middleware/         # JWT auth middleware
│   ├── models/             # Mongoose models (User, Ambulance, Item)
│   ├── routes/             # API, Auth & Admin routes
│   ├── server.js           # Express + Socket.io server
│   └── seedAdmin.js        # Admin seeder script
└── frontend/
    └── src/
        ├── components/     # Reusable UI components
        ├── layouts/        # Admin / Driver / Customer layouts
        ├── pages/          # Admin, Auth, Driver, Customer pages
        └── App.jsx         # Root app with routing
```

---

## 👥 Team

Built with ❤️ for Smart India Hackathon by Team ResQ.

---

## 📄 License

MIT
