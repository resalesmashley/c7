# Project Overview

## Development Commands
- Serve locally: `python3 -m http.server 8080`
- Format HTML/CSS/JS: use your editor's built-in formatter (no project-level tooling configured)

## Architecture Notes
- Single-page static experience built from `index.html`, styled via `style.css`, and driven by `script.js`.
- `script.js` handles all interactive flows (page switching, modals, cart logic) and stores demo data in plain objects and `localStorage` for persistence.
- Self-serve shop items live in the `SHOP_PRODUCTS` array, rendered dynamically with vanilla DOM APIs; parent/teacher/admin portal logic and mock data are defined in the same file.
- `style.css` contains global theme variables and layout rules for all sections, including responsive grids for portal pages and the self-serve shop.

## Data & Storage
- No backend or database; demo records (accounts, lesson plans, resources) are hard-coded in `script.js` and optionally cached in browser `localStorage` for persistence across reloads.
