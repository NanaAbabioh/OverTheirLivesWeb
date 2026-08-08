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

## Where the emails go ✅ (done)

The sign-up forms are wired to **Formspree** (endpoint `https://formspree.io/f/xaewqpoo`). When someone signs up, the address is captured by Formspree and emailed to **hello@overtheirlives.com**, and you can download the full founding-families list as a spreadsheet from your Formspree dashboard anytime.

**One-time activation:** the first time the form is used, Formspree emails you to confirm/activate the form — do one test sign-up on the live site, then click the confirmation link in that email. After that, all sign-ups flow automatically.

*Later, if you want to send fancier launch emails, you can export the Formspree list and import it into Kit/ConvertKit.*

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
