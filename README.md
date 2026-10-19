# 🗒️ Express.js Note Taker

A full-stack note-taking app with an Express.js back end that saves, retrieves, and deletes notes using a flat JSON file as a lightweight database. The front end is pre-built; this project focuses on the server-side routing and file system logic.


---

## 📖 Overview

This project wires a provided HTML/CSS/JS front end to a custom Express.js server. Notes are persisted to a `db.json` file using Node's `fs` module — no external database required. Each note gets a unique ID via an npm package, and a bonus DELETE route removes individual notes by ID.

---

## ✨ Features

- 📋 View all saved notes in the left-hand sidebar
- ✏️ Write new notes with a title and body
- 💾 Save notes — persisted to `db.json` via a `POST` route
- 🗑️ Delete notes by ID (bonus feature)
- 🔀 Express routing separates HTML and API concerns cleanly

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Runtime | Node.js |
| Server | Express.js |
| Persistence | `fs` module + `db.json` |
| Unique IDs | uuid (npm) |
| Deployment | Render |

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v18+)

### Installation

```bash
git clone https://github.com/Voobane/Express.js-Note-Taker.git
cd Express.js-Note-Taker
npm install
```

### Running the App

```bash
node server.js
```

Visit `http://localhost:3001` in your browser.

---

## 📁 Project Structure

```
Express.js-Note-Taker/
├── db/
│   └── db.json          # Note storage (auto-created/updated)
├── public/              # Pre-built front end (HTML, CSS, JS)
│   ├── index.html
│   ├── notes.html
│   └── assets/
├── routes/
│   ├── htmlRoutes.js    # GET / → index.html, GET /notes → notes.html
│   └── apiRoutes.js     # GET, POST, DELETE /api/notes
├── server.js            # Express setup and middleware
└── README.md
```

---

## 🔌 API Routes

| Method | Route | Description |
|--------|-------|-------------|
| `GET` | `/api/notes` | Return all saved notes as JSON |
| `POST` | `/api/notes` | Save a new note, return it with a unique id |
| `DELETE` | `/api/notes/:id` | Delete a note by its id (bonus) |

---

## 💡 What I Learned

- Setting up an **Express.js server** with static file serving and JSON middleware
- Separating routes into **HTML routes** and **API routes** for clean organization
- Reading and writing persistent data with **Node's `fs` module**
- Generating **unique IDs** with the `uuid` npm package
- Deploying a Node/Express app to **Render**

---

## 📸 Screenshots

> _Add screenshots to the repo and update this section._

---

## 👤 Author

**Matt (Voobane)**
- GitHub: [@Voobane](https://github.com/Voobane)
