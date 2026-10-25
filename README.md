# Amazon Warriors BJJ

Single-page website for Amazon Warriors Brazilian Jiu-Jitsu, San Antonio, TX.

## Stack
- Static HTML/CSS/JS, single file (`index.html`), no build step
- Fonts: Oswald + Source Sans 3 (Google Fonts)
- Logo and hero image are embedded as base64 data URIs

## Deploy (Cloudflare Pages)
1. Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git
2. Select this repo, production branch `main`
3. Build command: *(none)* · Build output directory: `/`
4. Custom domains → add the school domain, follow the DNS prompts

Every push to `main` redeploys automatically.

## Local preview
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Editing
All content (schedule, phone, address, programs, professor bio) lives in `index.html`. Search for the section `<!-- ... -->` comments or the `id=` anchors used by the nav.
