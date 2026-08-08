# Your website is built — read me first 🕊️

Hi Nana. The pre-launch site for **overtheirlives.com** is done and ready. Here's what it is, the **one thing left to wire up**, and exactly how to put it online.

---

## What was built

A single, self-contained page — `index.html` — that does one job: **collect emails from founding families** before the app launches Christmas Day 2026.

It has everything from the brief, top to bottom:

- **Hero** with your tent artwork, the *PRAY | SPEAK | DECLARE* line, "Prayers that know your child by name," and the first email sign-up.
- **The difference** — generic prayer cards vs. prayers with your child's actual name.
- **Body · Soul · Spirit** — three cards in coral, plum, and navy.
- **How it works** — three steps.
- **Be there Christmas morning** — a gentle live countdown to Dec 25, 2026, and the sign-up asked a second time.
- **Footer** — your logo, social icons, and a one-paragraph privacy note (opens when you click "Privacy").

It works on phones, tablets, and computers, and it's fast. Your original photos are untouched — the web-sized versions live in the new `assets/` folder.

---

## The ONE thing left to wire up: where the emails go

Right now, when someone signs up, the form shows the warm "You're in. See you Christmas morning. 🕊️" message — but **it isn't yet sending those emails anywhere.** You need to pick an email service, and then it's a one-line change.

**My recommendation (free and simplest): [Formspree](https://formspree.io)** — you sign up, it gives you a form web address, and every submission lands in your inbox. Later you can move to Kit/ConvertKit for fancier launch emails.

**How to connect it** (or send me the address and I'll do it):
1. Create a free form at your chosen service and copy its form address (a URL).
2. In `index.html`, find the text **`FORM_ACTION_PLACEHOLDER`** (it appears twice) and replace both with that URL.
3. Done — sign-ups now flow to you, and the page still shows the success message without reloading.

Until you do this, the form still *looks* and *feels* complete for testing — it just won't capture real addresses yet.

---

## How to put it online (about 10 minutes)

Easiest path — **Netlify Drop** (free, no account tricks):

1. Go to **[app.netlify.com/drop](https://app.netlify.com/drop)**.
2. Drag this whole folder's three website pieces onto the page: the `index.html` file **and** the `assets` folder. (Tip: drag the folder that contains both.)
3. Netlify gives you a live link instantly (like `something-lovely.netlify.app`) — check it on your phone.
4. To use **overtheirlives.com**: in Netlify, open **Domain settings → Add a custom domain**, type `overtheirlives.com`, and it will show you the exact DNS records to enter.
5. Log in wherever the domain is registered, and paste those records in. HTTPS (the padlock) turns on automatically.

Vercel and Cloudflare Pages work the same way if you prefer one of those.

> If you tell me **which email service** you want and **where the domain is registered**, I can wire the form and give you the exact DNS records to paste — just ask.

---

## Small decisions still yours to make ([NANA DECIDES])

- **Social links** — the footer icons currently point to the generic Facebook / Instagram / TikTok homepages. Send me your exact profile URLs and I'll set them.
- **Email service** — see above.
- **Analytics** — none added on purpose. Say the word if you ever want visitor stats.

Everything else is finished. 🎄
