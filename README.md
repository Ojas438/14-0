# 14–0 — Perfect Season cricket game

A single self-contained `index.html` (no build step, no dependencies). Draft an XI
across IPL eras (or play the Test / World Test Championship mode), then watch the
season simulate live. IPL season stats are real (2008–2024 ball-by-ball data).

## Deploy to Vercel — pick one

### A) Vercel CLI (no Git needed) — fastest
```bash
npm i -g vercel        # one-time
cd 14-0                # this folder (must contain index.html)
vercel                 # logs you in, creates a preview URL
vercel --prod          # promote to your production domain
```
When prompted: accept defaults; project name e.g. `14-0`; framework = **Other**.

### B) Drag & drop (no terminal)
1. Go to https://vercel.com/new
2. Choose **"Deploy"** → drag this whole `14-0` folder in (or its zip).
3. Framework preset: **Other**. Click **Deploy**.

### C) Git (auto-deploys on every push)
```bash
cd 14-0
git init && git add . && git commit -m "14-0 game"
# create an empty GitHub repo, then:
git remote add origin https://github.com/<you>/14-0.git
git push -u origin main
```
Then on vercel.com → **Add New → Project → Import** that repo → **Deploy**.

## Notes
- It's a static site: Vercel needs **no** build command and **no** output dir.
- `vercel.json` is optional (included only for clean URLs).
