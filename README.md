# TutorGuard

An AI-based cloud-native tutor management system.

## Stack

| Layer | Technology |
|---|---|
| Frontend | React (JavaScript) |
| Backend | Python + FastAPI |
| Database | PostgreSQL (AWS RDS) |
| AI | Amazon Bedrock + Python scoring |
| Hosting | AWS Amplify / Elastic Beanstalk |
| Auth | JWT (FastAPI) — Cognito later |

## Structure

- `client/` — React frontend
- `server/` — FastAPI backend
- `database/` — SQL migrations + seeds
- `infra/` — AWS deploy config
- `docs/` — SRS, ERD, API docs

## Getting Started

### Backend
```bash
cd server
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload
