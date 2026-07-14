# KW Southwest Newsletters

This repo hosts **two separate KW Southwest newsletters** on one domain:
`https://kwswnewsletter.brokermarketingdesk.com`. They are different products —
do not mix their content, styling, or folders.

## 1. Luxury Newsletter (dark / gold)

Dedicated luxury-listings email. Dark theme (`#0a0a0a`) with gold accent
(`#d4af37`), Playfair Display + Inter.

- **Location:** dated directories at the repo **root** (e.g. `jul-12-2026-newsletter/`,
  `may-27-2026-newsletter/`), each with a `newsletter.html`.
- **Shared assets:** `main-images/` (e.g. `kw-southwest-luxury.png`).
- ⚠️ **Do not move or rename these folders** — already-sent Luxury emails
  hot-link their images from these exact paths. Moving them breaks live emails.

## 2. General Monthly Newsletter (light / KW red)

General KW Southwest monthly newsletter. Light theme, KW corporate
red/black/white. Lives entirely under **`/monthly/`**.

- **Location:** `monthly/<issue-slug>/index.html`
  (e.g. `monthly/jul-14-2026-newsletter/index.html`).
- **URL:** `https://kwswnewsletter.brokermarketingdesk.com/monthly/<issue-slug>/`
- **Assets:** keep issue-specific assets inside each issue folder; shared
  general-newsletter assets go under `monthly/assets/`.
- One directory per monthly issue.

## Deployment

Static site on Vercel (project `kwsw-newsletter`). Pushing to `main`
auto-deploys. No build step.
