# hcp-ai-crm

# AI-Powered HCP Interaction CRM

## Project Overview

This project is an AI-powered CRM system for healthcare professional (HCP) interaction logging.

Users can describe interactions in natural language, and AI automatically extracts structured CRM data and fills the form.

Example:

"Met Dr Sharma at Apollo Hospital regarding insulin therapy. Positive discussion. Follow up Friday."

The AI extracts:
- HCP Name
- Interaction Type
- Date
- Time
- Products
- Topics
- Sentiment
- Outcomes
- Follow-up

---

## Tech Stack

### Frontend
- React
- Tailwind CSS
- Axios

### Backend
- FastAPI
- LangChain
- Groq LLM
- SQLAlchemy
- PostgreSQL (Neon DB)

---

## Features

- AI-powered interaction extraction
- Automatic form filling
- AI-based editing of logs
- Dynamic follow-up date generation
- PostgreSQL database integration
- FastAPI backend APIs

---

## Project Structure

```bash
frontend/
backend-hcp/
```

---

## Backend Setup

### Create virtual environment

```bash
python -m venv venv
```

### Activate environment

```bash
venv\Scripts\activate
```

### Install packages

```bash
pip install -r requirements.txt
```

### Run backend

```bash
uvicorn app.main:app --reload
```

---

## Frontend Setup

### Install dependencies

```bash
npm install
```

### Run frontend

```bash
npm run dev
```

---

## Environment Variables

Create `.env` file inside backend:

```env
GROQ_API_KEY=your_key
DATABASE_URL=your_database_url
```

---

## API Endpoint

POST `/ai/chat`

Example request:

```json
{
  "message": "Met Dr Sharma regarding insulin therapy"
}
```

---

## Author

Nikhil
