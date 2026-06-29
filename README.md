# Helium Studio — demo site

First-iteration marketing site. Static, hand-coded (HTML/CSS/JS, AI-assisted), zero build step. Deployed via GitHub → Vercel.

## Structure
```
index.html        the whole site (single file)
assets/           logo, favicons, work imagery
```

## Run locally
Just open `index.html` in a browser. (Or `python3 -m http.server` in this folder, then visit http://localhost:8000.)

## Deploy (GitHub → Vercel)
1. Create a new **empty** repo on github.com (e.g. `helium-demo`). Don't add a README/license.
2. In this folder, connect and push (the local repo is already initialised and committed):
   ```bash
   git remote add origin https://github.com/<your-username>/helium-demo.git
   git branch -M main
   git push -u origin main
   ```
3. On vercel.com → **Add New → Project** → import the repo.
   - Framework preset: **Other** · Build command: *(none)* · Output dir: `.` (root). It's static, so defaults are fine.
4. Deploy → you get a free `*.vercel.app` URL. Every `git push` auto-redeploys.

No custom domain for the demo (per the brief). Form is UI-only — no backend wired yet.

## Brand
Atmosphere gradient `135° #5B8DEF→#7C73F0→#9B6CF0` · violet dot `#7C73F0` · graphite `#1C2129` / `#0D1522`.
Fonts: Space Grotesk (headings), Hanken Grotesk (body), Space Mono (labels) — Google Fonts.
