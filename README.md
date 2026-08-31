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

Live at `https://<user>.github.io/<repo>/` in ~1 minute.

## Editing
Date, time, venue live in `index.html` — search for `13` / `11:00 AM` / `Thuruthi`.
Countdown target and calendar links are at the bottom of the file in the `<script>` block
(`2026-09-13T11:00:00+05:30` and `startUTC` / `endUTC`, which are UTC = IST − 5:30).
