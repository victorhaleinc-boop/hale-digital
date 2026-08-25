# BUILD BRIEF v2 — Hale Digital landing page (ANTI-AI-SLOP EDITION)

REBUILD index.html completely. Single self-contained file (inline CSS/JS, no frameworks).
The previous version failed because it looked AI-generated. This brief specifies EXACT
design tokens — follow them precisely. Deviation = failure.

## WHY THE OLD ONE FAILED (never do these)
Research on "why every AI website looks the same": purple/dark-navy gradient hero,
Inter-default font with no typographic identity, glowing buttons, three identical
cards in a row, emoji icons, glassmorphism, neon accents on black. ALL FORBIDDEN.
The target aesthetic is a WARM EDITORIAL paper feel (Notion-inspired) — light,
calm, expensive, human.

## DESIGN SYSTEM (use these EXACT values)

### Colors
- Page background: #ffffff
- Alternating section background: #f6f5f4 (warm white — has yellow undertone)
- Headings & body text: rgba(0,0,0,0.95) (near-black, NOT pure black)
- Secondary text: #615d59 (warm gray)
- Muted/captions: #a39e98
- Borders everywhere: 1px solid rgba(0,0,0,0.1) — whisper weight, never heavier
- ONE accent only: #0075de (CTAs, links, highlighted price). Nothing else saturated.
- CTA hover: #005bab. Focus ring: #097fe8.

### Typography (Google Fonts)
Primary: 'Source Sans 3' (weights 400,600,700) — body + UI.
Display/headings: 'Source Serif 4' (weights 600,700) — this is the identity font,
a serif headline on a trade-services page looks editorial and human, not AI.
- Hero H1: clamp(38px,6vw,64px), serif, weight 700, line-height 1.02, letter-spacing -2px
- Section H2: 40px serif 700, letter-spacing -1px, line-height 1.05
- Card titles: 21px sans 700, -0.25px
- Body: 16.5px sans 400, line-height 1.55, color rgba(0,0,0,0.95)
- Secondary text: 15px #615d59
- Badges: 12px 600, letter-spacing +0.3px, uppercase

Google Fonts link:
https://fonts.googleapis.com/css2?family=Source+Sans+3:wght@400;600;700&family=Source+Serif+4:opsz,wght@8..60,600;8..60,700&display=swap

### Depth (Notion-style, nearly invisible)
Card shadow: rgba(0,0,0,0.04) 0px 4px 18px, rgba(0,0,0,0.027) 0px 2px 7.85px,
rgba(0,0,0,0.02) 0px 0.8px 2.9px, rgba(0,0,0,0.01) 0px 0.175px 1.04px
Cards: white bg, whisper border, 12px radius. Featured card: 16px radius.
NO glow. NO colored shadows. NO backdrop-filter anywhere.

### Buttons
Primary: solid #0075de bg, white text, 4px radius (NOT pill), padding 10px 18px,
font 15px 600. Hover: #005bab. Active: scale(0.98). NO gradients, NO shadows on buttons.
Secondary: transparent bg, 1px rgba(0,0,0,0.1) border, near-black text. Hover: bg rgba(0,0,0,0.04).

## PAGE STRUCTURE (max-width 1140px centered, sections breathe 96px vertical)

1. NAV (white, thin bottom border): left = wordmark "Hale Digital" (serif 700, 19px,
   "Hale" normal + "Digital" in #0075de). Right: one primary button "Get my free audit".

2. HERO (white, 110px top padding): small pill badge above headline ("For South African
   plumbing businesses" — #f2f9ff bg, #097fe8 text, pill radius, 12px 600 uppercase).
   H1 (serif): "Every day your Google listing looks unfinished, someone else gets the call."
   Subline 20px 400 #615d59, max-width 560px: "We fix your Google presence, answer your
   reviews, and get you found — flat fee, done in 48 hours. No retainers, no agency games."
   Two buttons: primary "Get my free audit video" + secondary "See the two fixes".
   Below buttons: caption row 14px #a39e98: "48-hour delivery · Flat once-off fee · You own everything"

3. SOCIAL-PROOF STRIP (#f6f5f4 section): NOT stats-with-countups (AI tell). Instead one
   quiet sentence, centered, 17px #615d59 italic serif:
   ""87% of customers check Google before they call a tradesman. Most listings give them
   a reason not to.""
   Keep it humble. No fake numbers beyond this.

4. THE LEAK (white section): H2 "Where the calls are leaking". Then a NUMBERED EDITORIAL
   LIST (not cards!): three rows, each with oversized serif numeral (48px, #a39e98),
   bold title + one-sentence explanation, separated by whisper dividers:
   1. Unanswered reviews — "Customers read silence as 'closed down'. Competitors who reply look alive."
   2. Empty photo shelf — "Listings with 10+ photos get dramatically more direction requests. Most plumbers have three blurry ones."
   3. Wrong category setup — "You may not even appear for 'emergency plumber near me' — the highest-value search there is."

5. THE TWO FIXES (#f6f5f4 section): H2 "Two fixes. Two prices. Done."
   TWO cards side by side (asymmetric: featured card slightly larger/elevated):
   Card A (featured, white, 16px radius, subtle shadow, thin #0075de top border 3px):
     pill badge "Most popular", title "Google Visibility Rescue",
     price "R1 500" in 44px serif 700 with "once-off" caption, then 4 checklist lines
     (plain ✓ glyphs, not emoji), footnote "Live within 48 hours · Includes 30 days of review replies".
   Card B (white, standard): "Website Rescue", R2 500, checklist, footnote "Built, hosted, yours forever".
   Under both: 13px #a39e98 centered: "PayPal invoice · Half now, half on delivery available for first clients"

6. HOW IT WORKS (white): three steps as horizontal timeline with thin connector line,
   numbered circles (1px border, serif numerals): Free audit video → Flat-price fix →
   Live in 48 hours with before/after report. One sentence each.

7. FAQ (#f6f5f4): native <details> elements, whisper borders, serif questions at 18px.
   Q&A: guarantees (honest no + measurable fixes); who are you ("Independent. You deal
   directly with me, Mardan — my number, my work"); why so cheap (laptop overhead vs agency rent);
   payment (PayPal invoice, protected both sides); what if I hate it (before/after report, you keep everything either way).

8. FINAL CTA (white): H2 serif "Your next customer is searching right now." + primary button +
   caption "Free audit video. No strings."

9. FOOTER: whisper top border. Left: "Hale Digital — Google & web rescue for SA trades."
   Right: mailto link mardswar@gmail.com + wa.me/27649895786. Bottom line 13px #a39e98:
   "Serving plumbers & trade businesses across South Africa · Not for you? Reply STOP anytime."

## MICRO-INTERACTIONS (subtle only)
- Sections fade-up 12px on scroll (IntersectionObserver, 500ms ease-out, staggered 80ms) — ONCE, no loops
- Button hovers only change color/scale(0.98) — no glow, no shadow animation
- FAQ chevron rotates. NOTHING ELSE MOVES. Count-up animations are banned (AI tell).

## MOBILE (test at 375px mentally)
- Hero H1 → 34px, sections 56px padding, cards stack, timeline becomes vertical
- Sticky bottom bar: white bg, whisper top border, full-width primary button
  "Get my free audit video" + tiny caption under it. Hide when final CTA visible.

## COPY RULES
Plain SA English. Short sentences. Money-logic ("one emergency geyser job pays for this twice").
Never promise rankings. Never use words: unlock, elevate, seamless, supercharge, cutting-edge,
game-changer, empower. Zero emojis on the page. Zero exclamation marks.

DELIVERABLE: overwrite index.html in this folder. Single file. Nothing else.
