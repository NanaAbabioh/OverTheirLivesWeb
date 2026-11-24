# Over Their Lives — Website

The site for **[overtheirlives.com](https://overtheirlives.com)** — a mobile app that helps parents pray consistently and intentionally over their children. Launching **Christmas Day, December 25, 2026**.

## What's here

| File / folder | Purpose |
|---|---|
| `index.html` | The entire single-page site (self-contained: inline CSS + JS) |
| `terms.html`, `privacy.html`, `health-privacy.html` | Terms of Use, Privacy Policy and Consumer Health Data Privacy Policy. Served at `/terms`, `/privacy` and `/health-privacy` (static, no JS required). They share `assets/legal.css`. |
| `vercel.json` | `cleanUrls` config so those paths resolve with a 200 (no `.html`, no redirect chain). |
| `assets/` | Web-optimized images — hero, Open Graph card, favicon, logo mark |
| `WEBSITE-HANDOFF.md` | The original build brief |
| `READ ME — Website Built.md` | Plain-language notes: what's built, what's left to wire, how to deploy |
| `Logo OTL.png`, `OTL Banner Landscape.png` | Full-resolution source artwork |

## Tech

Plain static HTML — no framework, no build step. Deployable to any static host (Vercel, Netlify, Cloudflare Pages).

## Legal

The three legal pages are published at permanent addresses (`/terms`, `/privacy`, `/health-privacy`) to satisfy App Store / Google Play review and Apple Developer Program entity verification. They name **BLV Enterprises LLC** and its address; so does the footer on every page, which links to all three. The Privacy Policy directs rights requests to `privacy@overtheirlives.com` — keep that address receiving mail.

---
Over Their Lives · BLV Enterprises LLC · © 2026
