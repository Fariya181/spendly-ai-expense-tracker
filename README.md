# Spendly – Expense Tracker with AI Insights

Flask backend + single-page frontend. Expenses are stored in the browser (localStorage);
the backend only generates AI insights, so your API key stays on the server.

## Setup
```bash
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env            # then paste your key from console.anthropic.com
python app.py
```
Open http://127.0.0.1:5000

## Structure
- `app.py` – Flask server, `/api/insights` endpoint (rate-limited, size-capped)
- `static/index.html` – the UI
- `.env` – holds ANTHROPIC_API_KEY (never commit it)
