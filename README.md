# DukaanAI Starter — free single-shop demo

A responsive, installable web app starter for one small shop. It works on desktop and mobile browsers and can be added to a phone's home screen after publishing over HTTPS.

## Features included
- Dashboard with today's sales, estimated profit, stock count and low-stock alerts
- Product inventory: add, edit, search, delete, purchase cost, sale price, quantity and reorder threshold
- Sales recording: select a product, quantity and payment type; stock is deducted automatically
- Simple printable bill
- Sales history, CSV export, JSON backup
- Basic reports, top-selling products and rule-based shop tips
- Shop name, owner and phone settings
- Responsive mobile navigation and basic offline caching

## Important limitations
This is a **single-device prototype**, not a production multi-user system. Data is stored in browser `localStorage` on the current device. It does not yet have secure accounts, cloud sync, server database, online customer ordering, payment gateway, tax/GST-compliant invoicing or a real AI API. Do not store sensitive customer information in this prototype. Export backups regularly.

## Run locally
Open `index.html` in a browser. Some PWA/offline features require a local web server or HTTPS.

## Publish free with GitHub + Vercel
1. Create a GitHub account at https://github.com/signup
2. Create a new public repository, e.g. `dukaanai-starter`.
3. Upload `index.html`, `manifest.json`, `sw.js`, and `icon.svg` from this folder to the repository root.
4. Create a Vercel account at https://vercel.com/signup and choose **Continue with GitHub**.
5. Import the `dukaanai-starter` repository. Framework preset: **Other**; build command and output directory can be left empty/default for a static site.
6. Click **Deploy**. Vercel provides a free `*.vercel.app` address.
7. Open the URL on your phone. In the browser menu choose **Add to Home Screen** / **Install app** if available.

Free tiers and terms can change; check the current provider limits. A custom domain is not needed for the first demo.

## Updating
Edit the files on GitHub and commit the changes. Vercel automatically redeploys after a connected repository is updated.

## Suggested next production steps
1. Add authentication and a server-side database (e.g. Supabase free tier, subject to its current limits).
2. Add a proper customer order page and protected admin routes.
3. Add server-side validation, backups and access control.
4. Test stock, sales, export and restoration with the shopkeeper before using real business records.
