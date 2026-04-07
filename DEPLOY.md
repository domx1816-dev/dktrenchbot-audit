# DKTrenchBot v2 Audit Page — Deployment Guide

Your audit page is ready! Here are **3 deployment options** (easiest to most technical):

---

## Option 1: Cloudflare Pages (Recommended - Free, Instant)

1. Go to https://pages.cloudflare.com/
2. Click **"Create a project"** → **"Upload assets"**
3. Drag the `dktrenchbot-audit` folder into the upload box
4. Project name: `dktrenchbot-audit`
5. Click **"Deploy"**
6. You'll get a URL like: `https://dktrenchbot-audit.pages.dev`

**Time:** 2 minutes | **Cost:** Free

---

## Option 2: GitHub Pages (Free, Permanent)

1. Create a new public repo on GitHub (e.g., `dktrenchbot-audit`)
2. Upload `index.html` to the repo
3. Go to **Settings** → **Pages**
4. Source: **Deploy from branch** → `main` → `/ (root)`
5. Save
6. Your URL will be: `https://yourusername.github.io/dktrenchbot-audit/`

**Time:** 5 minutes | **Cost:** Free

---

## Option 3: Surge.sh (Fastest, but blocked on this server)

⚠️ Surge is blocked on this infrastructure (HTTP 451), but you can deploy from your local machine:

```bash
npm install -g surge
cd dktrenchbot-audit
surge . dktrenchbot-audit.surge.sh
```

**Time:** 1 minute | **Cost:** Free

---

## What's Included

- ✅ Single-page HTML file with full audit documentation
- ✅ Professional dark theme matching XRPL aesthetic
- ✅ Wallet addresses, strategy details, risk disclosures
- ✅ Performance projections and backtest data
- ✅ Source code structure and configuration parameters
- ✅ Responsive design (works on mobile)

---

## Quick Verification

Once deployed, verify these sections render correctly:
- Bot wallet: `rKQACag8Td9TrMxBwYJPGRMDV8cxGfKsmF`
- Main wallet: `rUWWnjZyBsmGPPLirtCf3NbUXJ1amet86e`
- Dashboard link: `https://dktrenchbot.pages.dev`
- GitHub repo: `https://github.com/domx1816-dev/dktrenchbot-v2`

---

## Need Help?

The archive `dktrenchbot-audit.tar.gz` contains everything needed for deployment. Just extract and upload to any static hosting provider.
