# Charlie Davidson — Personal Intranet

## Overview
This repository contains my personal intranet site: a lightweight place for projects, thinking, and exploration.

The site is intentionally split into two parts:
- a **public homepage** at `/` (personal bio / landing page)
- a **private dashboard** at `/dashboard/` for internal use

## Architecture
- **Hosting:** GitHub Pages
- **Application type:** static site (HTML, CSS, JavaScript)
- **Data model:** JSON-driven content (for example, travel locations)
- **Edge and access layer:** Cloudflare (DNS + Access)

## Access & Security
- The dashboard at `/dashboard/` is protected by **Cloudflare Zero Trust Access**.
- Authentication is handled with an **email-based one-time PIN**.
- Access is restricted to an approved email identity.
- Protection is enforced at the **Cloudflare edge**, before requests reach GitHub Pages.

## Project Structure
```text
/
├── index.html              # public bio page
├── dashboard/
│   └── index.html          # private dashboard
├── travel.html
├── photography.html
├── data/
│   ├── travel.json
│   └── photos.json
├── assets/
│   └── photos/
└── styles/
    └── main.css
```

## Features
- Public bio landing page
- Private dashboard behind Cloudflare Access
- Travel map with visited vs want-to-go locations
- Photography gallery
- Fast, lightweight static delivery

## Future Improvements

### UI/UX
- Improve spacing, typography, and visual hierarchy
- Add subtle animations and transitions
- Improve mobile responsiveness

### Travel
- Refine filters/toggles for visited vs want to go
- Add marker clustering
- Expand beyond the current top location set
- Add richer metadata (notes, dates, linked photos)

### Photography
- Add lazy loading for images
- Add lightbox/fullscreen viewing
- Add categorisation and tagging

### Dashboard
- Move to modular sections (cards/widgets)
- Add quick links and shortcuts
- Add personal notes or lightweight logs

### Security
- Keep access restricted to specific email identities
- Add/enforce MFA through Cloudflare Access
- Consider shorter session durations

### Technical
- Optionally introduce a lightweight build step (e.g. Vite)
- Extract reusable UI components (header, cards)
- Improve accessibility (contrast checks, ARIA labels)
- Add basic SEO metadata to the public page
- Add privacy-friendly analytics (e.g. Plausible)

### Performance
- Optimise images
- Improve caching strategy at Cloudflare
- Reduce JavaScript where possible

## Notes
This project is intentionally lightweight and evolving.

The focus is clarity, simplicity, and ownership—not over-engineering.
