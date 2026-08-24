# BUILD BRIEF — Hale Digital landing page

Rebuild index.html in this folder. Single self-contained file (all CSS/JS inline, no frameworks, no build step).

BUSINESS: "Hale Digital" — one-person digital studio in South Africa fixing Google presence for plumbing/trade businesses.

AUDIENCE: SA plumbing company owners, 35–60, browsing on phones between jobs. Skeptical of agencies. Motivated by lost revenue, not buzzwords. Plain talk wins.

PAGE GOAL: Get them to request a FREE 2-minute audit video of their own Google listing.
CTAs: email button mailto:mardswar@gmail.com?subject=Free%20audit%20video%20please and WhatsApp button https://wa.me/27649895786?text=Hi%2C%20I%27d%20like%20my%20free%20Google%20audit%20video
Secondary goal: prices feel like obvious no-brainers.

OFFERS (two cards side by side):
1. "Google Visibility Rescue" — R1 500 once-off. Full Google Business Profile overhaul, every review answered professionally within 24h for 30 days, competitor gap report, 30-day action plan. Delivered in 48 hours.
2. "Website Rescue" — R2 500 once-off. Fast modern one-page website with click-to-call and WhatsApp buttons, built and hosted, they own it forever.

REQUIRED SECTIONS (in order):
1. Hero: headline hits pain ("Every day your Google listing looks unfinished, someone else gets the call"), subline, dual CTA buttons, trust badges (48-hour delivery · flat fee · no retainers).
2. "The leak": 3 short punchy reasons plumbers lose calls on Google (no photos, unanswered reviews, wrong category). Big numerals or icons, generous whitespace.
3. Two premium pricing cards — recommended one visually highlighted, price as hero element of each card.
4. How it works: 3 steps (Free audit video → Flat-price fix → Live in 48h with before/after proof).
5. Stats band with count-up animation: "87% of customers check Google before calling · 2.7x more calls with 10+ photos · 0 retainers, ever".
6. FAQ accordion (details/summary fine): guaranteed rankings? (honest no — measurable fixes); who are you? (independent, deal with one person); how do I pay? (PayPal invoice upfront); what if I hate it?
7. Final CTA repeat + footer: "Hale Digital · Serving plumbers & trade businesses across South Africa · Not for you? Reply STOP anytime."

DESIGN DIRECTION:
- Premium dark theme: deep navy/near-black (#0B1220 range), ONE warm accent (amber #F5A524 range) used sparingly for prices/CTAs/highlights only. No gradient-everything, no purple AI slop.
- Distinctive display font from Google Fonts ("Sora", "Space Grotesk", or "Instrument Sans") + clean body font. Confident headline sizes, tight tracking on headings.
- Sections breathe (100px+ padding), cards subtle borders (#1E293B) + soft shadows, alive hover states.
- Micro-interactions: IntersectionObserver scroll-reveal fade+rise staggered; button hover transform+shadow; stats count-up. Vanilla JS under ~100 lines.
- Mobile-first, exceptional at 375px. Sticky bottom CTA bar on mobile ("Get my free audit video").
- Inline SVG logo mark for "Hale Digital" (abstract H or droplet+wrench hybrid, monochrome amber).
- Calm, expensive, fast — Stripe/Linear-adjacent adapted for blue-collar B2B.

COPY TONE: Short sentences. Zero jargon. Money-logic over marketing-speak. SA context welcome (geyser bursts, emergency call-out fees as job-value examples). NEVER promise Google rankings.

QUALITY BAR: This page is the product demo — it must look better than 95% of plumber websites, because clients judge the R2,500 Website Rescue by it. If a section feels like filler, cut it.

DELIVERABLE: overwrite index.html in this folder with the complete page. Do not create extra files.
