 Yatra Mitra AI — India Travel Chatbot

Yatra Mitra AI is a browser-based travel chatbot for destinations across India. It combines natural language intent detection (via configurable LLM providers) with client-side search over `Top Indian Places to Visit.csv` and automatic dataset fallback when the AI model is busy or fails.

## Overview

- **NLP + CSV Hybrid Routing:** Detects user intent, destination, starting city, trip days, travellers, hotel type, month, and language/script (including English, Hindi, Telugu, Tamil, and Hinglish), and checks `Top Indian Places to Visit.csv` when confidence is low, a place is missing, or the LLM request fails.
- **Travel Features:** Supports day-wise trip planning, INR trip budgets, destination comparisons, packing checklists, interactive maps (Leaflet/OpenStreetMap), destination photos (Wikipedia), live weather (Open-Meteo), reviews, and printable trip plans.
- **Tech Stack:** HTML, CSS, and vanilla JavaScript running on a local HTTP server.

## Project Structure

```text
yatra-mitra-ai/
├── index.html
├── Top Indian Places to Visit.csv
├── README.md
├── css/
│   └── style.css
└── js/
    ├── config.js
    ├── services.js
    ├── llm.js
    └── ui.js
