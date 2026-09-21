# karvachauth

Karva Chauth 2026 (Thursday, 29 October) — city-wise moonrise time site.
51 city pages + katha, sargi, vidhi, mehendi, songs guides.

## How it works
- `generate.js` computes sunrise/moonrise per city (suncalc, validated against Swiss-Ephemeris sources within ~1 min) and writes static HTML to `dist/`.
- GitHub Actions builds and deploys `dist/` to Cloudflare Pages → karvachauth.pages.dev.
- Requires repo secrets: `CLOUDFLARE_API_TOKEN`, `CLOUDFLARE_ACCOUNT_ID` (same as other SKM repos).

## Regenerate
npm install && node generate.js
