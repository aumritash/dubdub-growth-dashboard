# Dubdub Growth Dashboard

A single-file, self-contained growth dashboard for Dubdub — monthly acquisition
(cost-per-depth), paid channels (Meta / Google / Apple / Influencers / Collaborations),
community channels (Instagram / Reddit / WhatsApp / X / Discord), and an auto-generated
"What changed" digest with notes.

## Deploy

It's a static site — just `index.html`, no build step, no dependencies.

**Vercel (recommended):**
- Import this repo at [vercel.com/new](https://vercel.com/new) and deploy. No build command, no framework — Vercel serves `index.html` at the root automatically.
- Or from the folder: `npm i -g vercel && vercel --prod`.

## Data

Data is stored in each visitor's browser (localStorage) — nothing is uploaded.
Use **Data → Export JSON** to back up or hand off. To update the shared baseline
everyone sees, replace the seed data in `index.html` and redeploy.

Shared multi-person editing (Supabase or Google Sheets sync) can be added later
without changing the hosting setup.
