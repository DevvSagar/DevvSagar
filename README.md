# 👋 Hi, I'm Sagar Pratap Singh

🚀 Aspiring Software Engineer building secure, production-style backend systems and full-stack applications.

---

## 💡 About Me

* 🎓 BCA student at Career Point University, Kota
* 🔐 Focused on backend development with an emphasis on security — authentication, authorization, and data isolation done right, not just "it works"
* 🐍 Currently deep in Python/FastAPI, building REST APIs with JWT auth, PostgreSQL, and Alembic migrations
* 🚀 Learning by building — every project below is hand-built and tested, not copy-pasted from tutorials

---

## 🛠️ Tech Stack

* **Backend:** Python, FastAPI, Node.js, Express.js
* **Databases:** PostgreSQL, SQLAlchemy, Alembic
* **Frontend:** React, Tailwind CSS
* **Languages:** Python, JavaScript
* **Tools & Practices:** Git, GitHub, Docker, JWT Auth, REST API Design

---

## 🚀 Featured Projects

### 🔹 Scribo – AI Meeting Intelligence Platform
A full-stack application that transforms meeting recordings into structured transcripts and intelligent summaries.
* Built with React + Node.js
* Integrated AssemblyAI for AI-powered transcription
* Implemented secure backend practices (validation, rate limiting, sanitization)
* Designed for real-world usability and performance

👉 https://github.com/DevvSagar/scribo

---

### 🔹 Todo API – Secure REST API with Per-User Data Isolation
A FastAPI backend with JWT authentication, where every user only ever sees and modifies their own data.
* JWT-based auth: password hashing, token creation/verification, protected routes
* Per-user ownership enforced at the query level — tested by attempting cross-user access and confirming it's blocked
* PostgreSQL + SQLAlchemy, with Alembic-managed schema migrations
* Structured to industry convention (SQLAlchemy models vs Pydantic schemas cleanly separated)

👉 https://github.com/DevvSagar/Todo-FastAPI

---

### 🔹 Expense Tracker API – FastAPI Backend with Analytics
A personal finance tracking API extending the same secure auth pattern, with added query logic for real usage.
* Full JWT auth + per-user ownership, built independently after the Todo API
* Category filtering, total spend, and category-wise summary endpoints (aggregation queries)
* Recovered from and documented a real Alembic migration incident — diagnosed a stale import path that caused a bad schema drop, fixed it, and rebuilt the migration history cleanly

👉 https://github.com/DevvSagar/Expense-Tracker-API

---

## 📫 Connect With Me

* GitHub: https://github.com/DevvSagar
* LinkedIn: www.linkedin.com/in/devvsag

---

⭐ Continuously building, learning, and improving — one real bug at a time.
