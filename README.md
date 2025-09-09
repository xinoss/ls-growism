# ls-growism

**Lost Saga Training Simulation**  
A web-based tool for simulating character and equipment setups in ***KLS** Lost Saga*.

![App Screenshot](./assets/screenshot.png)

---

## ✨ Features
- **Hero & Equipment Simulation**: Test various character and gear combinations in real time.  
- **Cooldown & Stats Analysis**: Dynamically calculate cooldowns, stats, and performance.  
- **Visualization Tools**: Cooldown tables and stat charts for easier comparison.  
- **Utility Functions**: save/load system, and replay options for repeated testing.  

---

## 🛠 Tech Stack
| Layer        | Tech & Frameworks         |
|--------------|---------------------------|
| **Backend**  | Node.js, Express, MongoDB |
| **Frontend** | React (with TypeScript)   |
| **Language** | TypeScript / JavaScript   |

---

## 📂 Project Structure

```plaintext
ls-growism/
├─ backend/                # Backend (Node.js + Express + MongoDB)
│  ├─ src/
│  │  ├─ controllers/      # Request handlers
│  │  ├─ routes/           # API route definitions
│  │  ├─ models/           # Mongoose schemas & models
│  │  ├─ utils/            # Utility functions & helpers
│  │  └─ index.ts          # Entry point for the server
│  ├─ package.json
│  └─ ...
│
├─ frontend/               # Frontend (React + TypeScript)
│  ├─ src/
│  │  ├─ components/       # Reusable UI components
│  │  ├─ pages/            # Page-level components
│  │  ├─ hooks/            # Custom React hooks
│  │  ├─ services/         # API calls & data handling
│  │  └─ main.tsx          # Entry point for the app
│  ├─ package.json
│  └─ ...
│
├─ .env.example            # Environment variable template
├─ setupDB.js              # MongoDB template
└─ README.md
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/xinoss/ls-growism.git
cd ls-growism
```

### 2. Install dependencies

**Backend:**
```bash
cd backend
npm install
```

**Frontend:**
```bash
cd frontend
npm install
```

### 3. Setup environment variables

- **configure your MongoDB URI, server port, etc.** 

**Window:**
```bash
copy .env.example .env
```

**macOS / Linux:**
```bash
cp .env.example .env
```

### 4. Setup MongoDB 
```bash
cd database
mongoimport --uri "your_mongodb_uri" --db ls-growism --collection equipments --file equipments.json --jsonArray
mongoimport --uri "your_mongodb_uri" --db ls-growism --collection users --file users.json --jsonArray
```

### 5. Run the app

**Backend:**
```bash
npm run dev
# or
node index.js
# or
node .
```

**Frontend:**
```bash
npm run dev
# or
npm run build
```

---

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.  
