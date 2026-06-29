[README.md](https://github.com/user-attachments/files/29479058/README.md)
# the-better-earthlings# The Better Earthlings — Premium Lifestyle Website

A premium, 60fps-feeling, fully interactive website concept for The Better Earthlings — a sustainable lifestyle brand. Built with pure HTML, CSS, and JavaScript. Zero dependencies, zero APIs, zero cost.

![License](https://img.shields.io/badge/license-MIT-green.svg)
![Tech](https://img.shields.io/badge/tech-vanilla--js--css-blue.svg)
![Status](https://img.shields.io/badge/status-production--ready-brightgreen.svg)

---

## ✨ Live Demo

Open `index.html` in any modern browser. No server required.

```bash
# Simply open the file
open index.html

# Or serve locally (optional)
python3 -m http.server 8000
# Then visit http://localhost:8000
```

---

## 🎮 What's Inside

### 6 Interactive DIY Games

| Game | Description | Interaction |
|------|-------------|-------------|
| **♻ Waste Sorter** | Drag emojis into the correct bin (Recycle, Compost, Trash) | Mouse + touch drag, score tracking, visual feedback |
| **🌬 Mindful Breath** | 4-7-8 breathing technique synced to an animated circle | Start/stop, animated scale, countdown timer |
| **🌍 Carbon Calculator** | 5-question lifestyle quiz to discover your eco footprint | Progress bar, animated result bar, personalized tips |
| **🧠 Eco Memory** | Match 8 sustainability-themed emoji pairs | Card flip animation, move counter, shake on mismatch |
| **🌱 Plant Nurturer** | Grow a virtual plant with water, sunlight, and fertilizer | Animated stem growth, leaf blooming, flower at max level |
| **❓ Eco Quiz** | 5 knowledge questions with instant educational feedback | Correct/wrong highlighting, facts per answer |

### Premium Visual Features

- **Liquid Glass Navigation** — `backdrop-filter: blur(24px)` frosted glass effect
- **Animated Mesh Gradient Background** — 4 floating gradient orbs with CSS keyframe animations
- **Scroll Progress Bar** — Gradient line tracking page position
- **Intersection Observer Animations** — Elements fade up smoothly as you scroll
- **3D Phone Parallax** — Mockup tilts subtly with mouse movement
- **Floating Decorative Orbs** — Independent float animations with hover scale
- **Hover Micro-interactions** — Every card, button, and stat lifts and glows
- **Text Reveal Effects** — Gradient text transitions on scroll
- **Smooth Scroll** — Native CSS + JS anchor smooth-scroll

---

## 🗂️ File Structure

```
.
├── index.html          # Single self-contained file (HTML + CSS + JS)
└── README.md           # This file
```

> **Note:** Everything is contained in a single HTML file. No external assets, no build step, no package manager.

---

## 🎨 Design System

### Color Palette

| Token | Hex | Usage |
|-------|-----|-------|
| `--paper` | `#f8f7f4` | Page background |
| `--ink` | `#1a1f1c` | Primary text, buttons |
| `--sage` | `#8fa083` | Accents, highlights |
| `--olive` | `#4f6548` | Success states, primary green |
| `--moss` | `#1e2b1e` | Dark backgrounds, headings |
| `--sand` | `#e8dfcf` | Cards, icons, warm accents |
| `--clay` | `#b88362` | Terracotta accents |
| `--gold` | `#b9a16b` | Eyebrow text, decorative lines |
| `--muted` | `#6b756b` | Secondary text |

### Typography

- **Headings:** `DM Serif Display` — Editorial, elegant serif
- **Body:** `Inter` — Clean, modern sans-serif
- **Monospace/Numbers:** `Space Grotesk` — Stats, scores, timers

### Spacing & Radius

- Border radius: `32px` for cards, `999px` for pills/buttons
- Section padding: `90px` vertical
- Card gap: `20px–24px`
- Transition easing: `cubic-bezier(0.23, 1, 0.32, 1)` — smooth deceleration

---

## 🚀 Getting Started

### Prerequisites

Any modern web browser:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Installation

```bash
# Clone or download
git clone https://github.com/yourusername/the-better-earthlings.git
cd the-better-earthlings

# Open in browser
open index.html
```

---

## 🛠️ Customization

### Change Brand Colors

Edit the CSS `:root` variables at the top of the `<style>` block:

```css
:root {
  --paper: #f8f7f4;   /* Background */
  --ink: #1a1f1c;     /* Primary text */
  --sage: #8fa083;    /* Accent green */
  --olive: #4f6548;   /* Primary green */
  /* ... etc */
}
```

### Add More Game Items

**Waste Sorter:** Add to the `sortItems` array in the JavaScript:

```javascript
const sortItems = [
  { emoji: '📰', name: 'Newspaper', type: 'recycle' },
  { emoji: '🍌', name: 'Banana Peel', type: 'compost' },
  // Add more here...
];
```

**Memory Match:** Add to the `memoryEmojis` array:

```javascript
const memoryEmojis = ['🌿', '♻', '🌍', '💧', '🌳', '☀️', '🍃', '🔋'];
// Add more pairs (must be even number)
```

**Carbon Calculator / Quiz:** Add questions to the respective arrays following the existing structure.

---

## 📱 Browser Support

| Feature | Chrome | Firefox | Safari | Edge |
|---------|--------|---------|--------|------|
| Backdrop Filter | ✅ 90+ | ✅ 88+ | ✅ 14+ | ✅ 90+ |
| CSS Grid | ✅ | ✅ | ✅ | ✅ |
| Intersection Observer | ✅ | ✅ | ✅ | ✅ |
| CSS Custom Properties | ✅ | ✅ | ✅ | ✅ |
| Touch Events | ✅ | ✅ | ✅ | ✅ |

---

## 🏗️ Architecture

### Performance Optimizations

- **GPU-accelerated animations** — Only `transform` and `opacity` used for 60fps
- **Passive event listeners** — Scroll events use `{ passive: true }`
- **Intersection Observer** — Scroll animations don't run on every frame
- **CSS-only animations** where possible — No JS animation loop for background effects
- **Single file** — Zero HTTP requests, instant load

### Accessibility

- Semantic HTML5 elements (`<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- `aria-label` on decorative elements
- Focus states on all interactive elements
- Color contrast ratios meet WCAG AA standards
- Keyboard-navigable games (Tab + Enter/Space)

---

## 📝 License

MIT License — feel free to use, modify, and distribute.

```
Copyright (c) 2026 The Better Earthlings

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 🙏 Credits

- **Design & Development:** Inspired by Claude Fable 5 premium aesthetic
- **Fonts:** Google Fonts (DM Serif Display, Inter, Space Grotesk)
- **Icons:** Unicode emoji (no icon library dependencies)

---

## 📬 Contact

- **Email:** hello@thebetterearthlings.com
- **Phone:** +91 8017883733
- **Location:** Kolkata, India

---

> *"The new luxury is responsibility."* — The Better Earthlings
