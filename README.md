# Trippie — Clickable Wireframe Prototype

A self-contained, single-file clickable wireframe for **Trippie**, India's group trip planning app. Covers all 7 modules: Social, Survey, Discovery, Repository, Itinerary, Live Mode, and Expenses. No build step, no dependencies — `index.html` runs on its own.

## Deploy to GitHub Pages

1. **Create a repo** on GitHub (e.g. `trippie-prototype`). Keep it public, or use a private repo if your plan supports Pages.

2. **Add these files** to the repo root (this whole folder):
   - `index.html` — the prototype
   - `.nojekyll` — tells Pages to serve files as-is (don't skip this)
   - `README.md` — this file

   Via the web UI: open the repo → **Add file → Upload files** → drag in all three → **Commit**.

   Or via command line:
   ```bash
   cd trippie-prototype-site
   git init
   git add .
   git commit -m "Trippie clickable wireframe prototype"
   git branch -M main
   git remote add origin https://github.com/<your-username>/trippie-prototype.git
   git push -u origin main
   ```

3. **Enable Pages:** repo → **Settings → Pages** → under *Build and deployment*, set **Source = Deploy from a branch**, **Branch = main**, **Folder = / (root)** → **Save**.

4. **Wait ~1 minute**, then open:
   ```
   https://<your-username>.github.io/trippie-prototype/
   ```
   Share that link with anyone — no login required.

## Notes

- Everything is in `index.html` (HTML + CSS + JS inline), so it also works by double-clicking the file locally or opening from any static host (Netlify drop, S3, etc.).
- Toggle the **PRD requirement tags** overlay from the sidebar to trace each screen back to its requirement IDs.
- To update the deployed prototype, replace `index.html` and push again — Pages redeploys automatically.
