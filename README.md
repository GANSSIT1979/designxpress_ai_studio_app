# DesignXpress AI Studio Pro — Full‑Stack Web App (FastAPI + React)

Luxury **Gold + Black** themed creator suite for building content series, generating videos, and connecting social media accounts via OAuth.

## Stack
- **Backend:** FastAPI (Python), MongoDB (Motor), JWT auth (python-jose + passlib)
- **Frontend:** React + Router + TailwindCSS (+ optional shadcn-style components), Sonner toasts
- **Realtime:** WebSockets (video generation progress), with polling fallback

## Quick Start (Local Dev)

### 1) Backend
```bash
cd app/backend
cp .env.example .env
# set MONGODB_URI and JWT_SECRET_KEY at minimum
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
uvicorn server:app --reload --port 8000
```

### 2) Frontend
```bash
cd app/frontend
npm install
npm run dev
```

Frontend expects API at `http://localhost:8000` by default.

## OAuth Notes
OAuth providers are **optional**. Configure keys in `.env.oauth.example` and copy into `.env` when ready.

For local testing, ensure your provider console redirect URI matches:
- `http://localhost:8000/api/oauth/<provider>/callback`

## Project Layout
See `contracts.md` for API contracts and `USERS_MANUAL.md` for end‑user docs.
