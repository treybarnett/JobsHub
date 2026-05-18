# Qwick Jobs · Internal Launch Hub

Single-page GTM hub for the Qwick Jobs launch. Sales / CX / Ops / AM source-of-truth for product walkthroughs, docs, FAQ, and marketing assets.

## What's inside

- **Overview** — Hero positioning, key stats, content index
- **Loom Videos** — Sales Product Overview, CX Walk-through, Internal Product Walkthrough
- **Docs & Playbooks** — Foundational reading (Sales Briefing, Walkthrough v3, FAQ v3), Battlecard, 7-step Demo Playbook, FAQ
- **Marketing** — Marketing materials artifact + public qwick.com/jobs link

## Access gate

The page is gated by a simple client-side access phrase: **`QwickJobs`** (case-sensitive). The unlock persists for the browser session via `sessionStorage`. This is soft deterrence, not real security — the phrase is visible in page source.

## Deploy

It's a single self-contained `index.html` with zero build step. Any static host works.

### GitHub Pages (recommended)

1. Create a new repo on github.com (e.g. `qwick-jobs-hub`). Mark it private if you want.
2. From this folder:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-user-or-org>/qwick-jobs-hub.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
4. Wait ~30 seconds. Your site will be live at `https://<your-user-or-org>.github.io/qwick-jobs-hub/`.

> **Note on private repos:** GitHub Pages on a private repo requires a paid plan (Enterprise) for private Pages. On a free plan, the repo can be private but Pages will publish a public URL.

### Vercel / Netlify (alternative)

Drop the folder into Vercel or Netlify — no config needed. Both auto-detect static sites.

## Editing

All content (text, links, Loom IDs, doc cards, scenarios) lives in `index.html`. Open in any editor. No build, no install, no dependencies.
