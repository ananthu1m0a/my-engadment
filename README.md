# Aswathy & Ananthu — Engagement

Single-page static site. No build step, no dependencies.

**Event:** Sunday, 13 September 2026 · 11:00 AM · Thuruthi Temple Hall, Maradu

## Files
- `index.html` — whole site (HTML + CSS + JS inline)
- `assets/couple.jpg` — hero portrait
- `assets/invitation.jpg` — invitation card
- `assets/welcome.jpg` — welcome poster / social preview image
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Local preview
```
python3 -m http.server 8000
```
Open http://localhost:8000

## Deploy to GitHub Pages
```
git init
git add .
git commit -m "Engagement site"
git branch -M main
git remote add origin https://github.com/<user>/<repo>.git
git push -u origin main
```
Then: repo **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.

Live at https://ananthu1m0a.github.io/my-engadment/ in ~1 minute.

## Link previews
`og:image` / `og:url` in `index.html` are **absolute** URLs — WhatsApp, Facebook and
Twitter ignore relative ones. If the repo is renamed or moved to a custom domain,
update the four `https://ananthu1m0a.github.io/my-engadment/` references in `<head>`.

## Editing
Date, time, venue live in `index.html` — search for `13` / `11:00 AM` / `Thuruthi`.
Countdown target and calendar links are at the bottom of the file in the `<script>` block
(`2026-09-13T11:00:00+05:30` and `startUTC` / `endUTC`, which are UTC = IST − 5:30).
