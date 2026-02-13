# SKOOL Smart Intake

Conversational intake and survey tool for [SKOOL by MATANGA](https://matangaresearch.com) — AI productivity training for professionals.

## What This Is

An LLM-powered chat interface that replaces static forms with adaptive conversations. Two modes:

- **Intake** — Interview prospective students to understand their background, goals, and recommend a learning track
- **Survey** — Post-session reflection to capture learning outcomes and feedback

## How It Works

The page sends conversation history to an n8n webhook, which calls the Claude API with a system prompt and returns the response. All conversation state lives in the browser. The backend is stateless.

## Usage

Open `index.html` with a configured webhook URL:

```
index.html?mode=intake&webhook=YOUR_WEBHOOK_URL
index.html?mode=survey&module=NotebookLM&webhook=YOUR_WEBHOOK_URL
```

**Demo mode** (no backend needed):
```
index.html?demo=true
```

## License

Copyright MATANGA Research. All rights reserved.
