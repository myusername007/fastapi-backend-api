# FastAPI Backend API

Backend API built with **Python + FastAPI**, featuring **JWT authentication**, **PostgreSQL**, **SQLAlchemy**, and **Alembic migrations**.

## Features
- JWT auth (access/refresh)
- User management (CRUD)
- SQLAlchemy ORM + PostgreSQL
- Alembic migrations
- Clean project structure (routers/services/schemas)

## Tech Stack
- Python
- FastAPI
- SQLAlchemy
- PostgreSQL
- Alembic
- JWT

## Run locally

### 1) Create and activate venv
```
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
```
### 2) Install dependencies
```
pip install -r requirements.txt
```
### 3) Set environment variables
Create .env file:
```
DATABASE_URL=postgresql+psycopg2://user:password@localhost:5432/dbname
JWT_SECRET_KEY=your_secret
```
### 4) Apply migrations
```
alembic upgrade head
```
### 5) Run server
```
uvicorn app.main:app --reload
```

## API
Open Swagger UI:
/docs

## Notes
This project demonstrates backend API development with authentication, database integration, and clean architecture.
