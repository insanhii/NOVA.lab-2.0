# 🧪 NOVA.lab 2.0 - Interactive AI Laboratory Portal & Clinical AI Suite

> **SPPU 2024 Pattern Artificial Intelligence & Clinical AI Expert Systems Suite**  
> An interactive full-stack Web Application for simulating, visualizing, and analyzing AI algorithms, heuristic state-space searches, adversarial games, and expert systems.

---

## 🌟 Key Features

- **⚡ Interactive Visualizers**: Real-time step-by-step interactive simulations for classic AI problems.
- **📚 In-Depth Academic Manuals**: Comprehensive SPPU 2024 Pattern practical manuals, theory, algorithm steps, and mathematical formulations.
- **💻 Production-Ready Code Implementations**: C++ / Python / JavaScript standard algorithm implementations for all 10 practicals.
- **✍️ Interactive Self-Assessment Quizzes**: 5-question multiple-choice quizzes with instant feedback and score celebration effects.
- **🩺 Part-C Mini-Project**: Rule-based Medical Diagnosis Expert System with symptom tree evaluation and clinical disease inference.
- **📐 Mathematical & LaTeX Rendering**: Native support for mathematical formulations using KaTeX and GFM markdown rendering.

---

## 🔬 AI Practical Visualizers Suite

| # | Practical Title | Domain / Category | Visualizer Type |
|---|-----------------|-------------------|-----------------|
| 1 | **Reflex Agent for Vacuum Cleaner World** | Intelligent Agents | `vacuum` |
| 2 | **Tower of Hanoi** | State Space Representation | `hanoi` |
| 3 | **BFS Maze & Graph Pathfinder** | Uninformed Search | `bfs` |
| 4 | **A\* Search Algorithm (8-Puzzle)** | Informed Search / Heuristics | `eight-puzzle` |
| 5 | **Medical Diagnosis Expert System** *(Mini-Project)* | Knowledge Representation | `expert-system` |
| 6 | **Alpha-Beta Pruning** | Adversarial Search | `alpha-beta` |
| 7 | **BFS Robot Path Planning** | Uninformed Search | `bfs-robot` |
| 8 | **DFS Water Jug Problem** | Uninformed Search | `dfs-waterjug` |
| 9 | **8-Queens Problem (Backtracking)** | Constraint Satisfaction (CSP) | `eight-queens` |
| 10 | **Rule-Based Chatbot** | Natural Language Processing | `chatbot` |

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: [React 19](https://react.dev/) + [Vite 8](https://vitejs.dev/)
- **Routing**: React Router DOM v7
- **Styling & UI**: Custom CSS3, Lucide React Icons, Canvas Confetti
- **Mathematics & Markdown**: `react-markdown`, `remark-math`, `rehype-katex`, `remark-gfm`
- **HTTP Client**: Axios

### Backend
- **Runtime**: Node.js (ES Modules)
- **Framework**: Express.js 4/5
- **Database**: MongoDB (Mongoose ORM)
- **Environment**: Dotenv, CORS

---

## 📁 Project Structure

```text
nova-lab/
├── client/                     # Frontend Vite + React application
│   ├── public/                 # Static public assets
│   ├── src/
│   │   ├── components/         # Algorithm Visualizer components
│   │   ├── pages/              # Home & Assignment Detail views
│   │   ├── config.js           # API baseURL setup
│   │   ├── App.jsx             # Main router
│   │   └── main.jsx            # Entry point
│   ├── package.json
│   └── vite.config.js
├── server/                     # Backend Node.js + Express API
│   ├── models/                 # Mongoose schemas (Assignment.js)
│   ├── index.js                # Express API routes & SPA static server
│   ├── seed.js                 # SPPU 2024 dataset seeding script
│   ├── .env.example            # Sample environment variables template
│   └── package.json
├── package.json                # Root package for mono-repo management
└── README.md                   # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js**: v18.0.0 or higher
- **npm**: v9.0.0 or higher
- **MongoDB**: Local MongoDB instance or MongoDB Atlas Connection URI

---

### Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/insanhii/NOVA.lab-2.0.git
   cd NOVA.lab-2.0
   ```

2. **Install dependencies for Client & Server**:
   ```bash
   npm run install:all
   ```

3. **Configure Environment Variables**:
   Create a `.env` file in the `server` directory (`server/.env`):
   ```env
   PORT=5000
   MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/novalab_db?retryWrites=true&w=majority
   ```

4. **Seed the Database**:
   Populate MongoDB with the SPPU 2024 Pattern practical manuals and quizzes:
   ```bash
   npm run seed
   ```

---

## 🏃 Running the Application

### Option 1: Run Backend & Frontend Separately

- **Start Backend API Server** (Port 5000):
  ```bash
  npm run server
  ```

- **Start Frontend Dev Server** (Port 5173):
  ```bash
  npm run client
  ```

### Option 2: Full-Stack Production Mode
Build the client and serve via Express:
```bash
npm run build
npm run start
```

Open [http://localhost:5173](http://localhost:5173) (Dev) or [http://localhost:5000](http://localhost:5000) (Production) in your browser.

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/assignments` | Fetch summary list of all AI practicals |
| `GET` | `/api/assignments/:slug` | Fetch complete manual, code, quiz & metadata for a practical |

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 👨‍💻 Author

Developed with ❤️ by **[insanhii](https://github.com/insanhii)**
