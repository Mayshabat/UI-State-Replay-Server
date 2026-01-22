# UI State Replay Server (Flask + MongoDB)

Backend service for the **UI State Replay SDK**.

This server stores recorded UI sessions in **MongoDB Atlas** and exposes a REST API
to create, retrieve, update, and delete sessions.

---

## ✨ Tech Stack
- Python + Flask
- MongoDB Atlas (PyMongo)
- Flask-CORS
- Environment variables via `.env` (python-dotenv)

---

## ✅ API Base URL (Cloud)
If deployed on Render:

**Base URL:**  
https://ui-state-replay-sdk.onrender.com

---

## 🔌 Endpoints

- `GET /health` — Health check + DB connection
- `POST /sessions` — Create a new session
- `GET /sessions?limit=20` — List latest sessions (without events)
- `GET /sessions/{id}` — Get a specific session (including events)
- `PUT /sessions/{id}` — Update a session
- `DELETE /sessions/{id}` — Delete a session

---

## 📦 Local Setup

### 1) Install dependencies
```bash
pip install -r requirements.txt
```

## Run the server

python app.py
