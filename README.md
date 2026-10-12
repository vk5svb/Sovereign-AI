# Sovereign AI: the case for on-premise (Jyot)

A static, single-page site. No build step, no server, no external files needed.

## What is in this folder
- `index.html`  the whole page (fonts, map and images are inside it, about 0.7 MB)
- `favicon.svg`, `apple-touch-icon.png`  browser tab and iPhone home-screen icons
- `og-image.png`  1200x630 preview image for WhatsApp, LinkedIn, X
- `vercel.json`  clean URLs and basic security headers

## Deploy to Vercel (pick one)
**A. Through GitHub (recommended)**
1. Create a new GitHub repository and upload these files to its root.
2. On vercel.com choose Add New, then Project, and import the repository.
3. Framework Preset: Other. Leave Build Command and Output Directory empty. Click Deploy.
4. Every later change you push to GitHub redeploys automatically.

**B. Through the command line**
1. Install Node.js, then run: `npm i -g vercel`
2. In this folder run: `vercel` (follow the prompts), then `vercel --prod`

## After it is live
1. Add your domain: Project, Settings, Domains.
2. Link previews: open `index.html`, find the comment near the top that starts "After you know your final web address", and add the og:image line with your real address, for example
   `<meta property="og:image" content="https://your-domain/og-image.png">`
   Then push again. (WhatsApp and LinkedIn cache previews; use their debug tools to refresh.)
3. Do not want search engines to list it? Add `<meta name="robots" content="noindex">` inside `<head>`.

## Test before sharing
Open the live link on: an iPhone (Safari), an Android phone (Chrome), a Mac (Safari and Chrome), a Windows PC (Edge and Chrome). Check that the map zooms, pins open, the tabs switch, and the page scrolls smoothly past the map with your finger.

## Things to check
- Vercel's free Hobby plan is for personal, non-commercial use (donations do not count as commercial). Confirm the current terms for your organisation, or use another static host such as Cloudflare Pages.
- Confirm you may embed the Storica and Big Noodle Titling fonts on a public website. Montserrat and Jaini are open-licence.
- Content sign-off: the illustrative RBI and Article 370 boxes, the June-July 2026 suspension line, and entries marked as programmes or reported.
