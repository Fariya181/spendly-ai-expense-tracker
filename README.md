# Spendly – AI Expense Tracker

A personal finance web app that tracks daily expenses, monitors a monthly budget and generates AI-powered spending insights.

**Live demo:** https://your-app.onrender.com

## Features
- Add, delete and filter expenses by month
- Monthly budget tracker with progress bar
- Category breakdown donut chart
- AI insights from the Claude API (spending patterns, unusual items, saving tips)
- Export expenses to CSV
- Responsive UI with automatic light/dark mode

## Tech Stack
Python, Flask, Claude API (Anthropic), HTML, CSS, JavaScript

## Architecture
The frontend stores expenses in the browser (localStorage). The Flask backend exposes `/api/insights`, which sends the month's data to Claude and returns insights. The API key stays on the server.
