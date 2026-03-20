# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A static personal CV/portfolio landing page for Golicov Alexandr (Senior PHP Backend Engineer), hosted on GitHub Pages. No build tools, no package manager, no framework — pure HTML with Tailwind CSS via CDN. Kept intentionally simple to work with GitHub Pages static hosting.

## Development

**To preview:** open `index.html` directly in a browser, or serve with any static server:
```bash
python3 -m http.server 8080
```

**Deploy:** push to the `main` branch — GitHub Pages serves `index.html` automatically.

No build, lint, or test commands exist.

## Architecture

Single file: `index.html` (~290 lines). Four sections laid out top-to-bottom:

1. **Hero** — full-viewport gradient with profile photo, name/title, email + LinkedIn buttons, CSS fade-up animation
2. **Tech Stack** — tag cloud + 3-column grid (Backend / Databases / Infrastructure)
3. **Experience** — timeline of roles (2006–2026)
4. **Footer** — contact info

**Styling:** Tailwind CSS (CDN), custom `@keyframes` for fade-up and gradient animation, no custom JS logic.

**Assets:**
- `avatar.jpeg` — profile photo used in the hero
- `Golicov_Alexandr_CV_2026.docx` — downloadable resume linked from the page