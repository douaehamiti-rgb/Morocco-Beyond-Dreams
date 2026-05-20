# 🇲🇦 Morocco Beyond Dreams

> **A cinematic luxury tourism website showcasing the soul of Morocco — from the golden dunes of the Sahara to the blue streets of Chefchaouen.**

<div align="center">

### 🌐 [View Live Site](https://douaehamiti-rgb.github.io/Morocco-Beyond-Dreams/morocco-beyond-dreams.html)

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square&logo=github)](https://douaehamiti-rgb.github.io/Morocco-Beyond-Dreams/morocco-beyond-dreams.html)
[![HTML](https://img.shields.io/badge/HTML-Pure-orange?style=flat-square&logo=html5)](https://github.com/douaehamiti-rgb/Morocco-Beyond-Dreams)
[![CSS](https://img.shields.io/badge/CSS-Vanilla-blue?style=flat-square&logo=css3)](https://github.com/douaehamiti-rgb/Morocco-Beyond-Dreams)
[![JS](https://img.shields.io/badge/JavaScript-Vanilla-yellow?style=flat-square&logo=javascript)](https://github.com/douaehamiti-rgb/Morocco-Beyond-Dreams)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-red?style=flat-square)](https://github.com/douaehamiti-rgb/Morocco-Beyond-Dreams)

</div>

---

## ✨ Overview

**Morocco Beyond Dreams** is a premium single-page HTML/CSS website designed to evoke the beauty, culture, and luxury of Morocco through an immersive cinematic experience. Inspired by world-class travel brands and Awwwards-level design, every section tells a story.

---

## 🗺️ Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | **Hero** | Fullscreen cinematic background with Ken Burns effect, animated title, floating gold particles, and a bottom stats bar |
| 2 | **Destinations** | Interactive tabbed cards for 7 cities: Marrakech, Chefchaouen, Merzouga, Fès, Casablanca, Tangier, Agadir |
| 3 | **Natural Wonders** | Sahara Desert, Ouzoud Waterfalls, Dakhla Atlantic Coast with reveal-on-hover descriptions |
| 4 | **Culture** | Zellige, Khatt calligraphy, Tadelakt plaster, Andalusi music — text + 3-image mosaic layout |
| 5 | **Luxury Experiences** | 6 curated experience cards: Desert Camp, Riads, Gastronomy, Camel Tours, Surf, Hammam |
| 6 | **Gallery** | 9-photo masonry grid with cinematic hover captions |
| 7 | **Voices** | 3 glassmorphism testimonial cards with star ratings |
| 8 | **Booking** | Bespoke journey request form with styled inputs |
| 9 | **Footer** | Arabic branding, navigation links, social media |

---

## 🎨 Design System

### Color Palette

| Token | Hex | Usage |
|-------|-----|-------|
| `--black` | `#07070a` | Page background |
| `--gold` | `#c9a227` | Accents, borders, highlights |
| `--gold2` | `#e8c84a` | Hover states |
| `--sand` | `#d4b483` | Secondary text, card overlays |
| `--sand2` | `#ede0c4` | Primary body text |
| `--green` | `#1b4d3a` | Moroccan emerald accent |
| `--rose` | `#b06050` | Avatar gradients |
| `--cream` | `#f2e8d8` | Heading text |

### Typography

- **Cormorant Garamond** — Headings, pull quotes, large display text (serif, luxury feel)
- **Jost** — Body text, labels, navigation (geometric, clean)

### Effects & Animations

- Custom gold cursor with lagging ring follower
- Ken Burns zoom effect on hero background
- Floating gold particle system
- Parallax scrolling on hero image
- Intersection Observer scroll-reveal (fade up / fade left / fade right)
- 3D image hover with scale transform
- Glassmorphism cards (`backdrop-filter: blur`)
- CSS `animation` keyframes for loader, particles, pulse

---

## 📁 File Structure

```
Morocco-Beyond-Dreams/
│
├── morocco-beyond-dreams.html   # Complete site — single file
├── mosque-hassan.png            # Mosquée Hassan II photo (Casablanca tab)
└── README.md                    # This file
```

> All styles and scripts are **inline** inside the HTML file. No external frameworks, no bundler, no Node.js required.

---

## 🚀 Getting Started

### Option 1 — Open directly
```bash
# Just double-click the file, or:
open morocco-beyond-dreams.html
```

### Option 2 — Serve locally (recommended for best performance)
```bash
# Python
python3 -m http.server 8080

# Node.js
npx serve .

# VS Code
# Install "Live Server" extension → right-click → Open with Live Server
```

Then visit `http://localhost:8080`

---

## 🌐 Deployment

This is a **static site** — deploy anywhere for free:

### GitHub Pages
1. Upload your files to this repo
2. Go to **Settings → Pages**
3. Set Source to **Deploy from branch: main**
4. Click **Save**
5. Your site will be live at: `https://douaehamiti-rgb.github.io/Morocco-Beyond-Dreams/morocco-beyond-dreams.html`

### Netlify (drag & drop)
1. Go to [netlify.com](https://netlify.com)
2. Drag the project folder into the deploy zone
3. Done — live in seconds ⚡

---

## 📸 Images

All images are hosted on external CDNs or embedded directly in the HTML as base64:

- **External CDN** — Destination & experience photos loaded via URL
- **Embedded base64** — Mosquée Hassan II photo (works offline, no external dependency)

To replace any image, update the `src` attribute in the relevant `<img>` tag or swap the base64 string.

---

## 🔧 Customization

### Change hero background
```html
<!-- In CSS, find: -->
.hero-bg {
  background: url('YOUR_IMAGE_URL') center/cover no-repeat;
}
```

### Add a destination tab
1. Add a `<button class="dest-tab" data-tab="yourCity">` in the tabs row
2. Add a `<div class="dest-stage lay-2" id="tab-yourCity">` with card content

### Change the color scheme
All colors are CSS custom properties at the top of the `<style>` block — edit the `:root {}` section.

### Translate to French / Arabic
Replace all English text content in the HTML. The Arabic text `المغرب` in the footer is already present as a decorative element.

---

## ✅ Browser Support

| Browser | Support |
|---------|---------|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |
| Mobile (iOS/Android) | ✅ Responsive |

> `backdrop-filter` (glassmorphism) requires a modern browser. Firefox may need `layout.css.backdrop-filter.enabled` enabled in `about:config`.

---

## 📋 Features Checklist

- [x] Cinematic hero with Ken Burns + particles
- [x] Animated loading screen with progress counter
- [x] Custom gold cursor with ring follower
- [x] Scroll-reactive navbar (transparent → glassmorphism)
- [x] Interactive destination tabs (7 cities)
- [x] Hover reveal descriptions on all cards
- [x] Masonry photo gallery
- [x] Scroll-reveal animations (Intersection Observer)
- [x] Parallax hero background
- [x] Glassmorphism testimonials
- [x] Luxury booking form
- [x] Fully responsive (mobile, tablet, desktop)
- [x] Zero dependencies — pure HTML/CSS/JS
- [x] Single file — easy to deploy anywhere

---

## 🤝 Credits

- **Fonts** — Google Fonts (Cormorant Garamond, Jost)
- **Built with** — Pure HTML · CSS · Vanilla JavaScript

---

## 📄 License

This project is for **personal and portfolio use**. Photography credits belong to their respective owners. Please do not use commercially without replacing all third-party images with properly licensed alternatives.

---

<div align="center">

**Morocco Beyond Dreams** · مغرب ما وراء الأحلام

🌐 **[douaehamiti-rgb.github.io/Morocco-Beyond-Dreams/morocco-beyond-dreams.html](https://douaehamiti-rgb.github.io/Morocco-Beyond-Dreams/morocco-beyond-dreams.html)**

*Built with ❤️ and a love for Morocco*

</div>
