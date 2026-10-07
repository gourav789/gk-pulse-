# GK Pulse — Landing Site

Single-page marketing site for the GK Pulse current-affairs Telegram bot
(https://t.me/gourav_currentaffairs_bot). Built for Facebook/Instagram ads.

- `index.html` — the entire site (self-contained, no build step, no dependencies)
- `CNAME` — custom domain for GitHub Pages (`gkpulse.onl`)
- `robots.txt`, `sitemap.xml` — basic SEO

## Deploy on GitHub Pages

1. Create a new **public** GitHub repo (e.g. `gkpulse-site`).
2. Push these files to the `main` branch.
3. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` → `/root` → Save.
4. Under **Custom domain**, enter `gkpulse.onl` and Save (the CNAME file is already included).
5. At your domain registrar (where you bought `gkpulse.onl`), add DNS records:
   - Four `A` records for the apex domain `gkpulse.onl` pointing to GitHub Pages IPs:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - (Optional) a `CNAME` record for `www` → `<your-username>.github.io`
6. Wait for DNS to propagate (can take 10 min to a few hours), then enable
   **Enforce HTTPS** in Settings → Pages.

## Edit content

Everything is in `index.html`. Change the bot link, pricing, sources, or
languages directly in that file. No build needed — just edit and push.
