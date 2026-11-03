# Solar Power Install Website

Installation website for **SOLAR HE and Sons**. Fil Solar Depot sells the panels; this site is where customers book installation.

- **Live:** https://totoantonio.github.io/solarpowerinstall/
- **Repo:** https://github.com/totoantonio/solarpowerinstall
- **Sister site:** Fil Solar Depot → https://totoantonio.github.io/FilSolarDepot/ (source: `Documents/FilSolarDepot`)
- **Credit:** totoantonio.cloud (hidden in page meta: `designer`, `creator`, HTML comment)

## Stack
One `index.html` (styles + script inside) and `images/`. No framework, no build step. Font: Poppins (Google Fonts).

## Files
- `index.html` — the whole site
- `images/installer.jpg` — hero photo (free Pexels photo 8853504, replace with the real team)
- `images/og.png` — 1200×630 share preview image
- `images/favicon.svg`, `images/apple-touch-icon.png` — site icons
- `images/pagibig.svg`, `sss.svg`, `homecredit.png`, `gcash.svg` — "We Accept" logos (Wikimedia Commons)
- `images/surigao.png` — City of Surigao seal (Wikimedia Commons), sample client logo
- `images/bukidnon-1.jpg` to `bukidnon-10.jpg` — real installation photos, Malaybalay City, Oct 2026 (Commissioned sheet of `SolarHEandSons Page.xlsx`)
- `images/operations-manager.jpg` — crew with the Operations Manager, Cagayan de Oro, Oct 24, 2026 (OM sheet of the same file)

## Preview and publish
- Preview: `open index.html`
- Publish: commit and push to `main`; GitHub Pages rebuilds in about a minute.
- Facebook link preview cached? Use developers.facebook.com/tools/debug → Scrape Again.

## Theme (from the brand flyer)
| Use | Color | Hex |
|---|---|---|
| Primary, "SOLAR POWER." | Deep green | `#2F7D5B` |
| Headlines | Slate navy | `#2E3A4F` |
| Sun, accents | Sun orange | `#F6A21E` |
| Highlights, phone-bar Call button | Bright yellow | `#F5D33B` |
| Hero sky | Blue → sunset gold gradient | `#CFE3F5` → `#F8C77A` |

Headlines: Poppins Black Italic, highlighted word in green (yellow on the green booking section). Body: Poppins Regular.

## Page sections
1. Hero: headline, photo fading into the sky gradient, Book / Call buttons, "We Accept" logos (Pag-IBIG, SSS, Home Credit, GCash) level with the buttons; phones: text right-aligned, full-width buttons
2. Stats strip: TESDA, 50 Yrs, 1–3 Days, 500+
3. Why Homeowners and Businesses Choose Solar Power Install (4 cards)
4. Backed by HE & SONS + "#1 Top Solar Installer" panel
5. Our Services (6 cards)
6. How It Works (4 steps)
7. Commissioned in Bukidnon (`#projects`): uncropped photo gallery as proof of installation, 3 columns on desktop, 1 on phones; last photo has the one-line Operations Manager note
8. Book Your Installation form + contact details
9. FAQ
10. Trusted By: gray client logos rolling left to right in one line (marquee), not clickable
11. Footer; phone bottom bar (Call Us / Book Now)

Cards rise in on scroll and lift on hover. Layout checked from 320px to 1440px wide with no sideways overflow.

Navigation: at 900px wide or narrower the top links move into a hamburger menu. `scroll-padding-top` in the `html` style keeps section titles clear of the sticky header after a menu jump; update it if the header height changes.

## Still draft / need from the company
- Company name: headline says "Solar Power Install", logo/title/footer say "SOLAR HE and Sons" (decide later)
- Logo file (SVG or high-res PNG); current logo is redrawn from the flyer
- Real hero photo we have rights to use (hero is still the stock photo)
- Confirm permission for the live gallery photos: crew faces, client sites; `operations-manager.jpg` shows a street address and two readable license plates
- Email, address, service area, hours (draft: install@solarheandsons.com, Cagayan de Oro City, Mon–Sat 8 AM–5 PM). Also in the SEO data (JSON-LD in `<head>`), update both
- "500+ Systems Installed" (made up, marked "draft"), "1–3 days" install time
- Workmanship warranty term
- Installation prices or "quote after survey"
- Formspree ID `YOUR_FORM_ID` in the booking form (form doesn't send until set)
- Confirm Pag-IBIG, SSS, Home Credit, GCash are really accepted; use official logo files with permission
- Trusted By logos are SAMPLES (Surigao seal + Kibawe Farm + 8 made-up names). Replace with real clients, with permission
- Do not mention Blu Energy

## SEO / AI visibility
- `llms.txt` (summary for ChatGPT, Claude, Perplexity), `robots.txt` (all search and AI bots allowed), `sitemap.xml`
- Structured data (JSON-LD) in `<head>`: business profile + FAQ; geo tags for Cagayan de Oro
- On github.io, robots.txt and llms.txt only count at the domain root, so they take full effect after moving to a custom domain. Until then, submit `sitemap.xml` in Google Search Console and Bing Webmaster Tools
- Keep llms.txt and JSON-LD in sync when contact details, products or FAQ change
