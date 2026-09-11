# 🖥️ WEB-CLI-OS

> A web-based command-line operating system — built from the ground up with a React frontend, Node.js backend, and a C++ engine.

---

## 📦 Tech Stack

| Layer      | Technology            |
| ---------- | --------------------- |
| Frontend   | React.js              |
| Backend    | Node.js + Express     |
| Engine     | C++                   |
| Real-time  | WebSocket (Socket.io) |
| Storage    | File system / SQLite  |
| Deployment | Docker + CI/CD        |

---

## ⚙️ Setup

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- C++ compiler (`g++`)

### 1. Clone the Repository

```bash
git clone https://github.com/JayH25/WEB-CLI-OS.git
cd WEB-CLI-OS
npm install
```

### 2. Backend Setup

```bash
cd backend
npm install
cp .env.example .env
# Edit .env with your configuration
```

### 3. Frontend Setup

```bash
cd ../frontend
npm install
cp .env.example .env.local
# Edit .env.local with your configuration
```

### 4. Engine Setup

```bash
cd ../engine
g++ main.cpp -o main
```

### 5. Running the Application

```bash
# Start Backend (from /backend)
npm run dev

# Start Frontend (from /frontend)
npm start
```

- **Frontend:** http://localhost:3000
- **Backend API:** http://localhost:5000

### Environment Variables

**Backend (`/backend/.env`)**
| Variable | Default | Description |
|----------|---------|-------------|
| `PORT` | `5000` | Server port |
| `NODE_ENV` | `development` | Environment mode |
| `CORS_ORIGIN` | `http://localhost:3000` | Allowed frontend origin |

**Frontend (`/frontend/.env.local`)**
| Variable | Default | Description |
|----------|---------|-------------|
| `REACT_APP_API_URL` | `http://localhost:5000` | Backend API URL |
| `REACT_APP_NODE_ENV` | `development` | Environment mode |

---

---


> _Built with 🔥 by a team of 4 over 4–5 months. Every checkbox checked is one step closer to something legendary._
