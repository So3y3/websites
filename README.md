# Wee Sites

Static marketing site. Custom coded, no framework, no build step.

## Deploy to Vercel (free)

1. Create a new repo on GitHub (e.g. `wee-sites`) and push everything in this folder to it.
2. Go to vercel.com, sign in with GitHub, and click Add New Project.
3. Import the repo. Vercel auto-detects static sites, no config needed. Click Deploy.
4. Your site is live on a free `*.vercel.app` URL. Add a custom domain in Settings, Domains.

## Before you go live

Two placeholders need replacing:

1. **Formspree endpoint**: create a form at formspree.io, then in `index.html` replace
   `YOUR_ENDPOINT` in the form action with your new endpoint ID
   (`https://formspree.io/f/your-id`).
2. **Domain**: replace every occurrence of `www.weesites.co.uk` in
   `index.html` (canonical, og:url), `sitemap.xml` (loc), and `robots.txt`
   (Sitemap) with your real domain. If you keep the free vercel.app URL for now,
   use that instead so the sitemap stays valid.

## Files

- `index.html` — the whole site
- `404.html` — playful not-found page
- `sitemap.xml` — single URL, update after adding pages
- `robots.txt` — open to all crawlers
