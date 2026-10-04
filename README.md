# Architect + AI Engineering Mastery — Roadmap (PWA)

Installable, offline-capable study app. Progress is saved in your browser (localStorage).

## Run locally
```bash
python3 -m http.server 8080   # then open http://localhost:8080
```
(Service workers need `http://localhost` or HTTPS — they won't register from `file://`.)

## Deploy (GitHub Pages)
Push to `main`; the included workflow publishes the site.
One-time: **Settings → Pages → Source: GitHub Actions**.
Site URL: `https://<your-username>.github.io/<repo-name>/`

## Install
Open the site in Chrome/Edge/Android → *Install app*; on iOS Safari → *Share → Add to Home Screen*.

## Files
- `index.html` – the app (single file)
- `manifest.json`, – install metadata
- `sw.js` – offline caching (bump `VERSION` when you change files)
- `mermaid.min.js` – self-hosted Mermaid 11.17.2 so diagrams work offline
