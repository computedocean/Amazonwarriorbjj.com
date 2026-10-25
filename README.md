# Amazon Warriors BJJ

Single-page website for Amazon Warriors Brazilian Jiu-Jitsu, San Antonio, TX.

Live: https://amazonwarriorsbjj.com (Cloudflare Pages: https://amazonwarriorsbjj.pages.dev)

## Stack
- Static HTML/CSS/JS: `index.html` + `assets/` (logo, hero WebP, favicon, OG image), no build step
- Fonts: Oswald + Source Sans 3 (Google Fonts)
- SEO: meta description, Open Graph tags, LocalBusiness JSON-LD in `<head>`

## Deploy (Cloudflare Pages)
1. Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git
2. Select this repo, production branch `main`
3. Build command: *(none)* · Build output directory: `/`
4. Custom domains → add `amazonwarriorsbjj.com` and `www.amazonwarriorsbjj.com`

Every push to `main` redeploys automatically.

## Local preview
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Editing
All content (schedule, phone, address, programs, professor bio) lives in `index.html`. Search for the section `<!-- ... -->` comments or the `id=` anchors used by the nav.
