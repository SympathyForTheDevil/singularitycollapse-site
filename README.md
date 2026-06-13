# singularitycollapse.com

The marketing + legal website for **Singularity: Collapse**, a one-line cosmic
puzzle game. Static HTML/CSS, no build step, no dependencies — hosted free on
**GitHub Pages** with a custom domain.

## Pages
- `index.html` — landing page (hero, features, the collapse ladder).
- `privacy/` → **/privacy** — privacy policy. Matches what the app links to in
  Settings → About. ⚠ Update it if the app ever adds analytics or ads.
- `support/` → **/support** — support page + FAQ. Support email:
  `support@singularitycollapse.com`.
- `404.html`, `robots.txt`, `sitemap.xml`, `favicon.svg`.

## Hosting (GitHub Pages)
1. This repo is **public**; Settings → Pages → deploy from branch `main`, root `/`.
2. `CNAME` pins the custom domain `singularitycollapse.com`.
3. DNS (Namecheap): apex `A` records to GitHub Pages IPs + `www` `CNAME` to
   `<user>.github.io`. Enable **Enforce HTTPS** once the cert provisions.

## Notes
- Clean URLs (`/privacy`, `/support`) come from folder + `index.html`, so they
  work on any static host — these exact paths are referenced inside the app.
- Asset-free: the black hole is pure CSS/SVG, so there are no images to manage.
- The support email needs a working inbox — set up Namecheap email forwarding
  from `support@singularitycollapse.com` to your real address.
