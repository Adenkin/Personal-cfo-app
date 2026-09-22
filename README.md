# Personal CFO — Offline Phone App (Free)

A mobile-friendly **Progressive Web App (PWA)** version of the Personal CFO Financial Operating System.  
Works offline on your phone. **Zero cost** to run and install.

---

## What it includes

- **Dashboard** — Income, expenses, debt, net worth, emergency fund, DSR, status badge, alerts
- **Income** — Add / delete income entries
- **Expenses** — Track essential vs non-essential spending
- **Debt** — Register + Avalanche priority hint (highest interest first)
- **Savings & Emergency Fund** — Buckets, progress bars, coverage months
- **Net Worth** — Assets − liabilities
- **Goals** — Track progress toward targets
- **Settings** — Income, essential expenses, EF target, currency
- **Backup** — Export / import JSON (keep a copy safe)

All data is stored **only on your device** (browser localStorage). Nothing is sent to any server.

---

## Option A — Fastest (no account, no install tools)

### On Android (Chrome)

1. Copy the entire `personal-cfo-app` folder to your phone (USB, Google Drive, WhatsApp, etc.).
2. Open **Chrome** → menu → **Files** (or use a file manager) → open `index.html`.
3. Or: email the folder to yourself as a zip, download, extract, open `index.html` in Chrome.
4. Optional: Chrome menu → **Add to Home screen** / **Install app**.

### On iPhone (Safari)

1. Get `index.html` onto your phone (AirDrop, Files app, email, iCloud).
2. Open the file in **Safari**.
3. Tap **Share** → **Add to Home Screen**.
4. The app icon will appear on your home screen and open fullscreen.

> Note: Opening a pure `file://` page works for demos. For the best offline experience and “Install app” behaviour, use Option B (GitHub Pages) below.

---

## Option B — Best free method (GitHub Pages — recommended)

This gives you a real web address, proper offline caching, and “Add to Home Screen” that works reliably.

### Steps (all free)

1. **Create a free GitHub account**  
   https://github.com/signup

2. **Create a new repository**  
   - Click **New repository**  
   - Name it e.g. `personal-cfo`  
   - Set to **Public**  
   - Do **not** add a README if you will upload files yourself  
   - Create repository

3. **Upload the app files**  
   - In the new repo, click **Add file** → **Upload files**  
   - Upload everything from the `personal-cfo-app` folder:  
     - `index.html`  
     - `manifest.json`  
     - `sw.js`  
     - `icon-192.png`  
     - `icon-512.png`  
   - Commit

4. **Turn on GitHub Pages**  
   - Repo → **Settings** → **Pages** (left sidebar)  
   - Under **Source**, choose **Deploy from a branch**  
   - Branch: **main** (or master), folder: **/ (root)**  
   - Save  
   - Wait 1–2 minutes  

5. **Open on your phone**  
   Your app URL will look like:  
   `https://YOUR-USERNAME.github.io/personal-cfo/`  

6. **Install on phone**  
   - **Android Chrome**: open the URL → menu → **Install app** / **Add to Home screen**  
   - **iPhone Safari**: open the URL → Share → **Add to Home Screen**  

After the first visit, the service worker caches the app so it continues to work **offline**.

---

## Option C — Free alternatives to GitHub Pages

- **Netlify Drop**: https://app.netlify.com/drop — drag the folder, get a free URL (no account required for basic use in some cases; free account is fine).
- **Cloudflare Pages** / **Vercel** — free tiers, similar to GitHub Pages.

All of these cost **₦0**.

---

## Using the app

1. Open the app (browser or home-screen icon).
2. Demo data is pre-loaded so you can explore immediately.
3. Go to **More → Settings** and set your real monthly net income and essential expenses.
4. Replace demo income, expenses, debts, and savings with your figures.
5. Use **Export Backup** regularly and store the JSON file somewhere safe (Drive, email to yourself).
6. Status badge (Stable / Watch / Pressure / Critical) updates from your debt-service ratio and emergency-fund coverage.

---

## Important notes

- This is a **demo companion** to the Excel system, not a full replacement of every module.
- Not financial advice. Projections and status labels are guides only.
- Data lives in the browser on that device. Clearing browser data deletes it — use Export Backup.
- Never enter bank passwords, PINs, OTPs, or card CVVs into this app.

---

## File list

| File            | Purpose                          |
|-----------------|----------------------------------|
| index.html      | Full app (UI + logic + storage)  |
| manifest.json   | PWA install metadata             |
| sw.js           | Service worker (offline cache)   |
| icon-192.png    | App icon                         |
| icon-512.png    | App icon                         |
| README.md       | These instructions               |

---

## Updating later

Edit `index.html` on your computer, then re-upload the changed files to GitHub (or replace the file on your phone).  
If you use GitHub Pages, changes go live within a minute or two after you push.
