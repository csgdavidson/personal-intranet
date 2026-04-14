# Charlie HQ

Personal intranet for projects, thinking, and experimentation with AI-assisted coding.

Live: https://charliedavidson.co.uk

---

## Overview

This is a static site hosted on GitHub Pages, designed to evolve over time:

- **V1**: Static HTML, CSS, JavaScript
- **V2**: Serverless enhancements (Cloudflare Workers, auth)
- **V3**: Full personal platform (data, automation, AI workflows)

---

## Current Features

### Dashboard
- `index.html`
- Entry point to all projects
- Minimal, dark UI with project cards

### Travel
- `travel.html`
- Interactive map using Leaflet
- Displays visited vs planned destinations
- Stats summary (total / visited / want to go)

Data:
- `data/travel.json`
- Stores all travel locations with:
  - name
  - latitude / longitude
  - status (`been` or `want`)

---

## Project Structure
├── index.html
├── travel.html
├── data/
│ └── travel.json


---

## Tech Stack

- GitHub Pages (hosting)
- HTML / CSS / JavaScript (no framework)
- Leaflet.js (map rendering)
- OpenStreetMap tiles

---

## Design Principles

- Clean, minimal UI
- Dark theme
- Fast, static-first approach
- Separation of concerns (UI vs data)
- Iterative development (small safe changes)

---

## Next Steps

- Photography page (image grid)
- Travel filters (been / want toggle)
- Move more data to JSON
- Introduce authentication layer (Cloudflare Workers)

---

## AI Prompt Context (copy/paste for new chats)

Use this when starting a new ChatGPT/Codex session:

