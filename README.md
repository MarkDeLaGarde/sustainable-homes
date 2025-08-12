# Sustainable Homes — GitHub Pages

Static, single-file site for premium off-grid listings. Built to deploy on **GitHub Pages**.

## Quick start
1. Create a new repo, e.g. `sustainable-homes`.
2. Add this `index.html` (and the files in this folder).
3. Enable Pages: **Settings → Pages → Deploy from a branch → `main` / root**.
4. Wait for the green check, then visit `https://<your-username>.github.io/sustainable-homes/`.

## Editing listings
Open `index.html` and find `SH.data.listings`. Add or edit items:
- Set exactly **one** item with `premium: true` (pinned at top).
- For grid items, set `premium: false`.
- If a listing has **no images**, the “View photos” button is **hidden**.

## Custom domain
- Add a `CNAME` file with your domain, e.g. `sustainablehomes.au`.
- Point your DNS to GitHub Pages per Docs.

## SEO
- Canonical, Open Graph, and Twitter tags update automatically on route changes.
- `robots.txt` and `sitemap.xml` included. Replace `REPLACE_ME_BASE_URL` with your final URL.

## Forms
- Wired to **Formspree**. Update the endpoint in the `<form>` tag if needed.

## Development
All JS is in `index.html` under the `SH` namespace. The app is idempotent: re-initializing doesn’t duplicate UI or re-bind listeners.

---
© 2025 Sustainable Homes.
