# House of Miyou - Website Project

## Project Overview
Client website for **House of Miyou** (brand name: **La Belle Miyou**) — a Haitian food & beverage brand. This is a demo/presentation site built by rebranding an existing MIXSY cocktail template.

## Brand Details
- **Business Name:** House of Miyou
- **Brand Name (on labels):** La Belle Miyou
- **Phone:** 646-275-4540
- **Category:** Haitian beverages, spices, hot sauce, hair oil
- **Vibe:** Premium, warm, cream-colored aesthetic with gold and burgundy accents

## Products (with image filenames)
1. **Cremas Cocoye** — `images/cremas-cocoye.jpeg` — Cream-colored Haitian cremas (coconut, condensed milk, cinnamon, sugar). Bottles with gold caps.
2. **Liqueur Grenadine** — `images/liqueur-grenadine.jpeg` — Pink/rose Haitian liqueur. Bottles with gold caps on gold tray, served with cinnamon stick.
3. **Epis Lakay** — `images/epis-lakay.jpeg` — Traditional Haitian spice base in mason jars (yellow/green).
4. **Bon Piman** — `images/bon-piman.jpeg` — Haitian hot sauce in small bottles with red wax caps and twine tags. Two varieties (red and yellow).

## Products NOT yet on the site (mentioned by client but no images yet)
- Cremas Grenadia (grenadilla/passion fruit cremas)
- Hair Oil Coconut
- Additional spices

## Color Palette
```
--cream: #F5F0E8        (main background)
--cream-light: #FAF7F2  (section backgrounds)
--cream-dark: #E8E0D0   (subtle contrast)
--gold: #C5A55A          (buttons, highlights, accents)
--gold-light: #D4BA7A    (hover states, labels)
--gold-dark: #A68B3E     (card accents)
--burgundy: #7B2D3B      (hero bg, primary accent)
--burgundy-light: #9C3A4C
--burgundy-dark: #5A1F2B (hero gradient start)
--brown-dark: #3B2A1A    (footer bg, deep text)
--brown-warm: #6B4F3A    (secondary text)
--text-dark: #2B1F14
--text-light: #FAF7F2
```

## Typography
- **Headings/Brand:** Playfair Display (serif) — chosen over Bebas Neue for a more premium feel matching the label aesthetic
- **Body:** Inter (sans-serif)
- **Carousel headers:** Poppins loaded but Playfair Display used instead

## File Structure
```
mixsy-website/
├── index-v2.html          ← MAIN FILE (single-page site, everything inline)
├── images/
│   ├── cremas-cocoye.jpeg
│   ├── liqueur-grenadine.jpeg
│   ├── epis-lakay.jpeg
│   └── bon-piman.jpeg
├── components/            ← Original MIXSY component files (reference only, NOT used)
│   ├── hero-section.html
│   ├── about-section.html
│   ├── drinks-carousel.html
│   └── drinks-grid.html
├── hero-section.html      ← Original MIXSY files (reference only)
├── about-section.html
├── drinks-carousel.html
├── drinks-grid.html
└── CLAUDE.md              ← This file
```

## Site Sections (in index-v2.html)
1. **Loading Screen** — "HOUSE OF MIYOU" / "La Belle Miyou" text logo with burgundy-to-gold progress bar, "AUTHENTIC HAITIAN FLAVORS" footer text
2. **Navbar** — Fixed, glass effect on scroll. Logo: "HOUSE OF Miyou" (Miyou in italic). Links: Home, About, Products, Shop, Contact. Lang: EN/KR
3. **Hero Section** — Burgundy/brown gradient bg. Product slider (4 slides) with left info, center image, right ingredients. Gold floating particles. Arrow key navigation.
4. **About Section** — Cream bg. Curved SVG text "EVERY PRODUCT IS MADE WITH REAL INTENTION" with brown→burgundy→gold gradient. Two diagonal product images (cremas + liqueur) with "About Us" button.
5. **Products Carousel** — Horizontal scroll cards. "Discover Our *Finest* Haitian Flavors". 4 cards: Cremas (cream), Liqueur (rose), Epis (olive), Bon Piman (amber).
6. **Products Grid** — 3-column grid. Cremas Cocoye (cream card), Liqueur Grenadine (rose card), Bon Piman (gold card). Each with arrow button.
7. **Tagline Section** — Burgundy/brown gradient. "IT'S NOT JUST WHAT YOU [image] TASTE. IT'S WHERE IT TAKES *YOU*."
8. **Footer** — Dark brown bg. 4 columns: House of Miyou, Products, Support, Connect. Phone number. Instagram, Facebook, TikTok icons.

## What Was Done
- Took existing MIXSY cocktail website template and completely rebranded for House of Miyou
- Replaced all blue/pink color scheme with cream/gold/burgundy palette
- Swapped Bebas Neue font for Playfair Display serif
- Replaced cocktail glass loading animation with typographic brand logo + minimal progress bar
- Replaced all Unsplash stock images with actual product photos
- Changed floating blueberries to subtle gold floating particles
- Updated hero slider with 4 real products and their actual ingredients
- Updated carousel and grid with real product names and categories
- Changed footer from Twitter to TikTok, added phone number from bottle labels
- Added "EN / KR" language toggle (Kreyol)
- All product images sourced from client WhatsApp photos, stored in images/

## How to Run
```bash
cd "/Users/yoljean/Downloads/Ted Workspace/mixsy-website"
python3 -m http.server 8000
# Open http://localhost:8000/index-v2.html
```

## Known Issues / TODO
- No tagline yet (client hasn't provided one)
- Missing products: Cremas Grenadia, Hair Oil Coconut, additional spices (need images)
- All buttons currently show "Coming soon!" alert
- No actual e-commerce/ordering functionality
- Mobile menu button doesn't open a menu (just alerts)
- Images are raw WhatsApp photos — could be optimized/cropped for better presentation
- Original MIXSY component files still in repo (can be deleted once no longer needed for reference)
