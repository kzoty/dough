# Dough — Minimal PWA-ready site

This is a minimal Progressive Web App (PWA) skeleton intended to be published at:

https://kzoty.github.io/dough

Files added:

- `index.html` — simple welcome page, registers the service worker and supports install prompt
- `manifest.json` — web app manifest referencing the included icons
- `sw.js` — basic service worker that caches the app shell for offline use
- `icon-192.png`, `icon-512.png` — provided icons (already in repo root)

How to publish (GitHub Pages):

1. Commit and push these files to the `gh-pages` branch or to the repository root on the `main` branch, then enable Pages in repository settings.
2. Ensure `index.html` and the icons are at the repository root (or at `/dough` path if using a project page). For your URL `https://kzoty.github.io/dough` push into a repository named `dough` and enable GitHub Pages.

Testing PWA locally:

- Open the site in Chrome or Edge, open DevTools > Application and check Manifest and Service Worker sections.
- Use Lighthouse (Audits) to verify PWA installability and offline support.

If you want a cache-busting strategy, offline fallback page, or more advanced runtime routing, tell me which features to add.
