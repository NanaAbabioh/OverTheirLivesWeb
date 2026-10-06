# Over Their Lives — Pre-Launch Website

The pre-launch waitlist site for **[overtheirlives.com](https://overtheirlives.com)** — a mobile app that helps parents pray consistently and intentionally over their children. Launching **Christmas Day, December 25, 2026**.

## What's here

| File / folder | Purpose |
|---|---|
| `index.html` | The entire single-page site (self-contained: inline CSS + JS) |
| `privacy.html` | Privacy Policy for the mobile app. Served at `https://overtheirlives.com/privacy` (static, no JS required). |
| `vercel.json` | `cleanUrls` config so `/privacy` resolves with a 200 (no `.html`, no redirect chain). |
| `assets/` | Web-optimized images — hero, Open Graph card, favicon, logo mark |
| `WEBSITE-HANDOFF.md` | The original build brief |
| `READ ME — Website Built.md` | Plain-language notes: what's built, what's left to wire, how to deploy |
| `Logo OTL.png`, `OTL Banner Landscape.png` | Full-resolution source artwork |

## Tech

Plain static HTML — no framework, no build step. Deployable to any static host (Vercel, Netlify, Cloudflare Pages).

## Before it captures real emails

The sign-up form is wired to Formspree; submissions go to `hello@overtheirlives.com`.

## Legal

`privacy.html` is the app's Privacy Policy, published at `https://overtheirlives.com/privacy` to satisfy App Store / Google Play review and Apple Developer Program entity verification. It names **BLV Enterprises LLC** and its address; so does the footer on every page. The policy directs rights requests to `privacy@overtheirlives.com` — keep that address receiving mail.

---
Over Their Lives · BLV Enterprises LLC · © 2026
