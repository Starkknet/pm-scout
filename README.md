# 🧭 PM Scout

> **AI-powered copilot that finds remote Product Management internships, ranks them, applies automatically, and emails hiring managers — with a live tracker & reminders.**

---

## 🚀 Features (MVP Goals)
- **Job Aggregation** — Ingest postings from Greenhouse, Lever, Ashby, Workday, etc.
- **Relevance Ranking** — Filter by keywords, domain (SaaS/AI/Fintech), remote option, and experience level.
- **Auto Apply Bot** — One-click apply for Greenhouse/Lever forms (with resume tailoring & prescreen Q&A bank).
- **Cold Outreach** — Generate personalized emails/LinkedIn DMs to hiring managers.
- **Application Tracker** — Kanban-style board to track status and deadlines.

---

## 🛠️ Tech Stack
**Backend:**
- FastAPI (Python)
- PostgreSQL (with SQLAlchemy ORM)
- Celery + Redis (async tasks)
- Playwright (browser automation)

**Frontend:**
- Next.js (React + TypeScript)
- Tailwind CSS + shadcn/ui components

**Infra:**
- Docker + Docker Compose
- Hosted on Vercel / Fly.io / Supabase (planned)

---

## ⚙️ Local Development Setup
```bash
# 1. Clone the repo
git clone https://github.com/<your-username>/pm-scout.git
cd pm-scout

# 2. Copy environment variables
cp .env.example .env

# 3. Start services (Postgres DB for now)
cd ops
docker compose up -d
