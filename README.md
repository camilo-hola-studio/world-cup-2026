# 🏆 FIFA World Cup 2026 — Live Dashboard

A fast, responsive dashboard for the 2026 FIFA World Cup. Shows Round of 32 fixtures with Melbourne AEST kick-off times, full group standings, Golden Boot race, records, and fun facts. English/Spanish toggle.

**Live site:** [Add your Vercel URL here after deployment]

## Stack

- Plain HTML + CSS + JS — zero build step, zero dependencies
- Hosted on Vercel (free tier, global CDN)
- ESPN public API for live score refresh (no API key required)

## Features

- **Fixtures** — all 16 Round of 32 matches with Melbourne AEST times, venues, and confirmation status
- **Bracket** — full knockout bracket from R32 to the Final
- **Groups** — all 12 group tables with qualification status
- **Golden Boot** — top scorers with all-time World Cup goal records
- **Tournament Stats** — overview numbers and host nation details
- **EN / ES language toggle** — full bilingual support
- **Live Melbourne clock** — always shows current AEST time
- **Live ticker** — scrolling news and records

## Local development

No build step needed. Just open `index.html` in a browser:

```bash
open index.html
# or
python3 -m http.server 3000
```

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → New Project → Import from GitHub
3. Select this repo — Vercel auto-detects static site, no config needed
4. Click Deploy → live in ~30 seconds

Every `git push` to `main` auto-deploys.

## Data updates

Match data is embedded in `index.html` inside the `MATCHES`, `GROUPS`, and `SCORERS` arrays. Update these as results come in. Round of 32 results will be confirmed after June 27 (last group matches).

## Roadmap (post-MVP)

- [ ] Pull live scores from ESPN public API automatically
- [ ] Push notifications for match kick-offs (Web Push API)
- [ ] Round of 16 / QF / SF bracket auto-update
- [ ] Player stats deep-dive pages

## Credits

Data sourced from public match records. Not affiliated with FIFA.
