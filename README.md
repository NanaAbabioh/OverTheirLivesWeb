# Over Their Lives — Pre-Launch Website

The pre-launch waitlist site for **[overtheirlives.com](https://overtheirlives.com)** — a mobile app that helps parents pray consistently and intentionally over their children. Launching **Christmas Day, December 25, 2026**.

## What's here

| File / folder | Purpose |
|---|---|
| `index.html` | The entire single-page site (self-contained: inline CSS + JS) |
| `assets/` | Web-optimized images — hero, Open Graph card, favicon, logo mark |
| `WEBSITE-HANDOFF.md` | The original build brief |
| `READ ME — Website Built.md` | Plain-language notes: what's built, what's left to wire, how to deploy |
| `Logo OTL.png`, `OTL Banner Landscape.png` | Full-resolution source artwork |

## Tech

Plain static HTML — no framework, no build step. Deployable to any static host (Vercel, Netlify, Cloudflare Pages).

## Before it captures real emails

The sign-up form is complete but not yet wired to an email provider. Search `index.html` for `FORM_ACTION_PLACEHOLDER` (appears twice) and replace with your form endpoint (e.g. Formspree, Kit, Mailchimp). See `READ ME — Website Built.md` for full instructions.

---
Over Their Lives · BLV Enterprises LLC · © 2026
