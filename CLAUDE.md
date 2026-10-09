# scharenbergs.com

Personal site for Bryon Scharenberg. Static single page served by GitHub Pages from `main` (custom domain in `CNAME`).

## Structure

- Everything lives in `index.html`: styles, markup, and script.
- Most photos are embedded as base64 `data:` URIs, so the file is large. Do not read it whole. Use grep to find the section you need, then read only those lines. Images used in more than one place are separate files in the repo root (e.g. `smart-cookies-panel.jpg`).
- Sections in page order: hero, `expertise`, `smartcookies`, `experience`, `tools`, `story`, `thinking`, `life`, `contact`. Proof comes before personal narrative; keep the nav in the same order.
- Mobile overrides live in the `@media (max-width: 900px)` block in the `<style>` tag. Inline `grid-template-columns` styles need an `!important` override there or they overflow on phones.

## Workflow

- Never commit to `main` directly. Work on a branch and open a pull request. Merging to `main` publishes the site.
- Show a diff before committing.
- Preview locally with `python3 -m http.server 8000` from the repo root, then open http://localhost:8000. Embedded Spotify and YouTube players work there; they may not when opening the file directly.
- This repo is public, and GitHub Pages serves every file in it, including this one. Keep anything private out of the repo.

## Writing rules

- Plain, warm, first-person voice. Short sentences.
- No em dashes. No emojis. No performed enthusiasm or hype words ("unlock", "seamless", "game-changing").
- Avoid three-item rhythm lists and punchy sentence fragments.
- When featuring other people (panelists, guests), they are the interesting part. Credit them by name and title.

## Accuracy rules

- Never invent or inflate a metric, title, or level of involvement.
- Titles and claims must match the CV:
  - Director of Growth & GTM Strategy, Kalles Group (May 2022 to present)
  - Head of Recruiting & Marketing, Kalles Group (Aug 2019 to May 2022)
  - Recruiting Manager, Kalles Group (Oct 2018 to Aug 2019): 5 direct reports, 400+ interviews, 30+ hires
  - Smart Cookies: helped launch it (2024); designs each program, preps panelists, moderates every panel
  - $0 to $5M is cumulative revenue over three years, with 150% YoY growth in one year
- If a new claim can't be traced to the CV or a public source, ask before adding it.
