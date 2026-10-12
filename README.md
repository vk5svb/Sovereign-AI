# Sovereign AI for the Global South (Jyot): full-screen presentation site

A static site. No build step, no server, no external files. It is a 16-slide, full-screen
presentation with Previous / Next buttons (also keyboard arrows, swipe, a Contents menu and
per-slide links such as /#9 for the map). The VK 5.0 / Jyot header banner sits at the top of every slide.

## Files
- `index.html`   the whole site (fonts, map, logos are inside it, about 0.8 MB)
- `favicon.svg`, `apple-touch-icon.png`   tab and iPhone home-screen icons
- `og-image.png`   1200x630 link-preview image for WhatsApp, LinkedIn, X
- `vercel.json`   clean URLs and basic security headers

## Deploy to Vercel (pick one)
A. GitHub (recommended): create a repository, upload these files to its root, then on vercel.com
   choose Add New > Project > import it. Framework Preset: Other. Leave Build Command and
   Output Directory empty. Deploy. Pushing to GitHub later redeploys automatically.
B. Command line: `npm i -g vercel`, then in this folder run `vercel` and later `vercel --prod`.

## After it is live
1. Add your domain: Project > Settings > Domains.
2. Link previews: in `index.html`, find the comment "After you know your final web address" and add
   `<meta property="og:image" content="https://YOUR-DOMAIN/og-image.png">`, then push again.
3. Optional: add `<meta name="robots" content="noindex">` in the head to stay out of search engines.

## Test before sharing
iPhone (Safari), Android (Chrome), Mac (Safari, Chrome), Windows (Edge, Chrome). Check: Next/Previous
and swipe; the Contents menu; the map (pins, zoom, region buttons, layer switch); and the quiz.

## What is inside (16 slides)
1 Cover, 2 Three truths, 3 Three things you cannot outsource, 4 Where does your data go?, 5 What cannot leave the room,
6 Governments have already said no (official notices restricting AI), 7 Prohibition is not a strategy (the cost of "no",
with an interactive calculator), 8 The Global South is building its own, 9 World map (sovereign builds, where a
sovereign stack fills the gap, per country and per domain, plus value traditions), 10 The sovereign stack,
11 Each nation's own values, 12 How the value layer is built, 13 Five questions, 14 What you stand up, 15 See it in
January, 16 About and sources.

## Things to check
- Vercel's free Hobby plan is for personal, non-commercial use (donations are not commercial under
  Vercel's guidelines). Confirm current terms for your organisation, or use another static host.
- Confirm you may embed the Storica and Big Noodle Titling fonts on a public site. Montserrat and
  Jaini are open-licence.
- Map: India as officially depicted by the Government of India (Natural Earth India point of view,
  public domain, simplified for world scale). Other boundaries are as in that dataset.
- Content sign-off: the illustrative RBI and Article 370 boxes, the June-July 2026 suspension line,
  and the country entries. Each reported item has a source on the final slide.
- The "stack fit" lines per country and domain are Jyot's assessment, not descriptions of any institution's current practice.
- The calculator is illustrative arithmetic from the UK government trial's self-reported 26 minutes a day (about 13 working days a year); it is not a forecast.
