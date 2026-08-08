# OVER THEIR LIVES — One-Page Website Handoff
*Read this first. It is the complete brief for building overtheirlives.com. Follow it as written; where a decision is left open it is marked **[NANA DECIDES]**. Do not invent new messaging — all copy is provided below.*

---

## 1. What this is

A single-page pre-launch website for **Over Their Lives**, a mobile app that helps parents pray consistently and intentionally over their children. The app launches **Christmas Day — December 25, 2026**. Until then, this page has exactly ONE job: **capture emails** ("founding families" waitlist). Every design decision serves that job. No blog, no multiple pages, no navigation beyond anchor links.

**The product in one line:** personalized prayers for your children — during onboarding parents enter their child's name, age, and gender, and every prayer in the app's catalog is personalized with that child's name. Not generic prayer cards: *their* child's name inside every prayer, covering the child's **body, soul, and spirit**.

## 2. Brand context

- **Name:** Over Their Lives (BLV Enterprises LLC)
- **Anthem line (Nana's own, use verbatim):** PRAY | SPEAK | DECLARE over their lives
- **Positioning:** the prayer app for parents praying over their children. Warm, faith-filled, judgment-free. The enemy is inconsistency and parental guilt — the brand is the gentle answer, never the accuser.
- **Voice rules:** invitation, never guilt ("never miss a day" energy, not "if you don't pray…"). Not preachy. Scripture used sparingly and precisely. Prayers can happen ANY time of day — do not frame the brand as bedtime-only.
- **Core symbol:** a tent — the covering over a family — with warm light glowing inside and a parent leading a child by the hand into the light. Hero artwork is provided (see Assets).

### Colors
| Role | Hex |
|---|---|
| Midnight (dark backgrounds) | #0B0F1A |
| Deep Night (gradient partner, derived from brand navy) | #1C2A42 |
| Brand Navy — "Spirit" | #3D5A80 |
| Soft Plum — "Soul" | #7B2869 |
| Warm Coral — "Body" | #E07A5F |
| Doorlight Gold (accents, glow, CTAs) | #E3A94F |
| Candle Cream (light text on dark) | #F6EFE2 |

Gold is rationed: glow, key accents, and the primary CTA button only. Body/Soul/Spirit colors identify the three dimensions in Section 4 of the page.

### Typography
- Headings / display: **Cormorant Garamond** (Google Fonts), 500–600 weight
- Body / UI: **Jost** (Google Fonts), 300–500 weight
- If Nana supplies different fonts in this folder, hers win.

## 3. Page structure & copy (top to bottom)

All copy below is approved draft — polish rhythm if needed but do not change meaning or add hype language ("revolutionary", "game-changing" are banned).

### A. Hero (full viewport)
- Background: the provided 16:9 hero artwork (tent glowing in an open field). Dark gradient scrim as needed for text legibility. If artwork file is missing, use a midnight-navy gradient (#0B0F1A → #1C2A42) with a soft gold radial glow rising from the bottom edge — do NOT substitute stock imagery or AI-generate a replacement.
- Eyebrow (small caps, gold): `PRAY | SPEAK | DECLARE`
- H1: `Prayers that know your child by name.`
- Subline: `Over Their Lives helps you pray over your children consistently and intentionally — personalized prayers for their body, soul, and spirit. Launching Christmas Day 2026.`
- Email capture form (see Section 4 below): single email field + button. Button label: `Become a Founding Family`
- Under-form microcopy: `Free to join. First prayers arrive Christmas morning.`

### B. The problem → the difference (short section)
- H2: `You've prayed the prayers that say "insert your child's name here."`
- Body: `Prayer cards and graphics are everywhere — and they're generic. Over Their Lives is different: tell us your child's name once, and every prayer in the app becomes theirs. The same prayer you pray tonight carries your child's name, not a blank line.`

### C. Body · Soul · Spirit (three cards)
- H2: `Cover all of them. All of it.`
- Card 1 — **Body** (coral accent #E07A5F): `Health, protection, sleep, growth. Prayers for the child you can hold.`
- Card 2 — **Soul** (plum accent #7B2869): `Mind, emotions, friendships, courage. Prayers for who they're becoming.`
- Card 3 — **Spirit** (navy accent #3D5A80): `Faith, identity, purpose. Prayers that lead them to God.`

### D. How it works (three steps)
1. `Tell us about your child` — name, age — that's all we need.
2. `Choose today's prayer` — a growing catalog for every season and situation: first days of school, sickness, friendships, fear, milestones.
3. `Pray, speak, declare` — every prayer personalized with your child's name. Any time of day. Every day.

### E. Founding Families (the ask, repeated)
- H2: `Be there Christmas morning.`
- Body: `The app arrives December 25, 2026 — our gift to your family. Founding families get early access on Christmas Eve, a founding-family badge in the app, and launch-week perks. It costs nothing to join the list.`
- Repeat email form.

### F. Footer
- Small mark/logo (provided in Assets), social icons linking to: facebook.com/ [Nana's page], Instagram, TikTok — **[NANA DECIDES: exact profile URLs]**
- Line: `Over Their Lives · BLV Enterprises LLC · © 2026`
- Privacy note (required, we collect emails): link to a simple privacy page or inline modal — one honest paragraph: emails used only for launch updates, never sold, unsubscribe anytime. Children's names are NOT collected on this website.

### Optional (nice-to-have, only if it stays clean)
- A subtle countdown to December 25, 2026 in section E.
- A gentle scroll-triggered glow animation on the hero. No parallax circus; the page should feel calm.

## 4. Email capture — technical

- **[NANA DECIDES]** which email service. Ranked recommendation:
  1. **Kit (formerly ConvertKit)** — free tier, built for creators, easy launch broadcast later. Embed its form or POST to its API.
  2. **Beehiiv / Mailchimp** — fine alternatives if she already has an account.
  3. **Formspree** — if she just wants emails in an inbox for now (fastest, migrate later).
- Until she chooses: build the form UI complete with a clearly marked `FORM_ACTION_PLACEHOLDER` and validation, so wiring the provider is a one-line change.
- Form must: validate email client-side, show a warm success state (`You're in. See you Christmas morning. 🕊️`), never redirect off-page, work on mobile.

## 5. Technical requirements

- Single-page static site. Prefer ONE self-contained `index.html` (inline CSS/JS) unless there's a strong reason otherwise. No frameworks, no build step — this must be trivially hostable anywhere.
- Mobile-first responsive; test at 375px, 768px, 1440px. Most traffic will come from Instagram/Facebook/TikTok bio links on phones.
- Fast: compress/scale the hero image (≤ 400KB target for the web version), lazy-load anything below the fold, system font fallbacks while Google Fonts load.
- SEO/meta: title `Over Their Lives — Prayers That Know Your Child by Name`; meta description from hero subline; Open Graph + Twitter card tags using the hero art (create a 1200×630 OG crop from it); favicon from the provided mark.
- Accessibility: real labels on the form, alt text, contrast-checked text over imagery.
- Analytics: **[NANA DECIDES]** — default to none at launch; add later if asked. Do not add trackers unprompted.

## 6. Hosting & domain

- Domain owned: **overtheirlives.com** (currently linked from the Facebook page).
- Deploy path: any static host works. Recommended: Vercel or Netlify free tier — drag-and-drop or CLI deploy, then point the domain (A/CNAME per host's instructions) at it. Cloudflare Pages equally fine.
- **[NANA DECIDES]** where the domain is registered; the session doing deployment should ask her for registrar access or hand her the exact DNS records to paste.
- HTTPS required (automatic on all hosts above).

## 7. Assets expected in this folder

| File | Status |
|---|---|
| Hero artwork 16:9 (tent in field, daylight) | **Nana will add** — use the highest-res file present; filename will contain "hero" or "banner" |
| Logo / mark (square, transparent) | **Nana will add** |
| Night version of tent artwork (optional alternate) | may be present |
| `Over Their Lives — Social Media Strategy.docx` | context: full brand & growth strategy |
| `DOORLIGHT — House Format v1.html` | context: visual format system for social content |

If the hero or logo file is missing when you build: build everything with the documented fallbacks and clearly tell Nana which files to drop in and where they'll appear.

## 8. Definition of done

1. `index.html` in this folder, opening flawlessly on phone and desktop.
2. Every section above present, copy as specified, brand colors and fonts correct.
3. Form validates and shows the success state (placeholder action clearly marked if provider not yet chosen).
4. OG/meta tags in place with the OG image generated.
5. A short plain-language note to Nana: what was built, the one thing left to wire (form provider), and the exact steps to deploy + point the domain.

## 9. What NOT to do

- No multi-page site, no menus, no "About us" sprawl.
- No stock photography, no AI-generated replacement art — the provided artwork is the brand.
- No guilt-based copy, no countdown-pressure dark patterns beyond the gentle Christmas countdown.
- No collecting anything beyond email on this site (no children's names here).
- No newsletter popups. One page, one ask, asked twice.

---
*Prepared August 2026 in the Over Their Lives strategy session. Full strategy and brand rationale live in the companion files in this folder.*
