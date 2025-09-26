# AI Agent for Capital Markets News Sentiment Analysis and Summary

A web-based system to analyze financial news, provide concise summaries, and deliver sentiment analysis (positive/neutral/negative) for faster market insights.

## Features

- Input financial news articles via the web UI
- Get instant AI-generated news summaries
- See sentiment analysis (label + score)
- Results available in text and JSON formats

## Project Structure

- `backend/` : FastAPI backend with Azure GenAI integration
- `frontend/` : React web frontend
- `docs/` : Technical design and documentation
- `data/` : Sample articles for testing

## Quick Start

### Backend

```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
# Edit .env with your Azure GenAI API key
uvicorn app.main:app --reload
```

### Frontend

```bash
cd frontend
npm install
npm start
```

---

## API

- `POST /analyze`: Analyze article, returns summary & sentiment

---

## References

- Azure GenAI, FastAPI, React.js