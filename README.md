# Maniflask — Brand Site

Maniflask is the manifestation water bottle: your western zodiac on the bottle, your goals on a sticker, your ritual in every sip. This repo is the marketing landing page (static, no build step).

## Deploy (GitHub → Vercel, same stack as stwadd.com)

1. Import this repo in Vercel (account already linked to GitHub): `New Project → Import Git Repository → chinaselection-01/maniflask`.
2. Framework preset: *Other* (static). Root directory: `/`. No build command, no output dir.
3. Project Settings → Domains → add `maniflask.com`, then add the DNS records Vercel shows at your domain registrar (CNAME → `cname.vercel-dns.com`).

## Before go-live checklist

- [ ] Replace `YOUR_FORM_ID` in `index.html` (waitlist form) with your Formspree form ID.
- [ ] Replace `YOUR_COMMUNITY_FORM_ID` (Manifestations Wall form) with your Formspree form ID.
- [ ] Fonts load from Google Fonts CDN (Playfair Display + Inter) — needs internet at runtime.

## Files

- `index.html` — the site (self-contained: inline CSS + SVG, no external assets except webfonts + Formspree).
- `vercel.json` — static deploy config.
- `.vercelignore` — keeps PDF / print files out of the web deploy.
- `Maniflask_插卡_英文版_A4.pdf`, `插卡_英文版_印刷稿.html`, `包装设计.html` — print/box design source, not part of the site.
