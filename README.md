# Pranav Vaidhya — Portfolio Website

**Advanced CSS3 & Responsive Architecture**
*JavaScript Logic & State Management — Internship Assignment Task 2*

---

## 📋 Project Overview

A fully responsive, modern portfolio website built using **HTML5 and CSS3 only** (with minimal JavaScript for interactive features). The project demonstrates mastery of advanced CSS3 techniques including CSS Grid, Flexbox, custom CSS variables, light/dark mode, animations, and mobile-first responsive design.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🌗 Dark/Light Mode | CSS variables + JS toggle, saved to localStorage |
| 📐 CSS Grid Layout | Used for hero, about, portfolio, services, footer sections |
| 📦 Flexbox | Used for navbar, buttons, cards, social icons, form |
| 📱 Mobile-First | Responsive from 320px to 4K screens |
| 🎬 Scroll Animations | IntersectionObserver reveal animations on scroll |
| 📊 Animated Skill Bars | Skill progress bars animate when scrolled into view |
| ⏳ Loading Screen | Elegant loader on page entry |
| 🔝 Scroll-to-Top | Floating button appears after scrolling down |
| 🧭 Sticky Navbar | Transparent → frosted glass on scroll |
| 🍔 Hamburger Menu | Mobile-friendly sliding navigation |
| 💎 Glassmorphism | Glass-effect cards with backdrop-filter blur |
| ✨ CSS Animations | keyframes: float, pulse, blink, reveal, orb effects |
| 🖋️ Gradient Text | CSS gradient on hero name using background-clip |
| 📬 Contact Form | Functional with success feedback |
| 🎨 Custom Scrollbar | Styled scrollbar via ::-webkit-scrollbar |
| 📏 CSS clamp() | Fluid responsive typography throughout |

---

## 🗂️ Website Sections

1. **Navbar** — Sticky, responsive, with theme toggle and hamburger menu
2. **Hero** — CSS Grid layout with animated code window and stats
3. **About** — Two-column grid with floating avatar card
4. **Skills** — Auto-fit grid with animated progress bars
5. **Services** — 4-column responsive grid with hover effects
6. **Portfolio/Work** — Project cards with live demo + GitHub links
7. **Testimonials** — Glass-effect quote cards
8. **Contact** — Side-by-side grid with form and info
9. **Footer** — 3-column grid with links and copyright

---

## 🛠️ Technologies Used

| Technology | Usage |
|---|---|
| **HTML5** | Semantic structure, sections, forms, data attributes |
| **CSS3** | All styling — Grid, Flexbox, Variables, Animations |
| **CSS Grid** | Page layouts, hero, portfolio gallery, footer |
| **Flexbox** | Navbar, buttons, cards, social icons |
| **CSS Variables** | Light/dark theme system via :root |
| **@keyframes** | Loader, float, reveal, orb, tag-blink animations |
| **backdrop-filter** | Glassmorphism effects on cards and navbar |
| **CSS clamp()** | Fluid responsive typography |
| **IntersectionObserver** | Scroll reveal + skill bar trigger (JS) |
| **localStorage** | Theme preference persistence (JS) |
| **Google Fonts** | Playfair Display + Outfit font pairing |

---

## 📐 CSS Architecture

### CSS Custom Properties (Variables)
All colors, spacing, and effects are defined as CSS variables in `:root` for the dark theme, and overridden in `[data-theme="light"]` for light mode. This enables instant theme switching with a single attribute change.

```css
:root {
  --bg: #0a0c12;
  --accent: #c8f55a;
  --text-1: #f0f2f8;
  /* ... */
}
[data-theme="light"] {
  --bg: #f5f6fa;
  --accent: #5a8f00;
  /* ... */
}
```

### CSS Grid Usage
- **Hero section**: `grid-template-columns: 1fr 1fr` — content left, code window right
- **About section**: `grid-template-columns: 1fr 1.6fr` — avatar left, content right
- **Skills/Portfolio**: `repeat(auto-fit, minmax(280px, 1fr))` — auto-responsive columns
- **Footer**: `grid-template-columns: 2fr 1fr 1fr` — brand + two link columns

### Flexbox Usage
- Navbar: `display: flex; justify-content: space-between`
- Buttons: `display: inline-flex; align-items: center; gap: 8px`
- Cards: internal alignment of icons, text, and actions
- Social icons: horizontal row with gap

### Mobile-First Media Queries
```css
/* Base styles = mobile */
/* Tablet adjustments */
@media (max-width: 1024px) { ... }
/* Mobile */
@media (max-width: 768px)  { ... }
/* Small mobile */
@media (max-width: 480px)  { ... }
```

---

## 🚀 How to Run Locally

### Option 1 — VS Code Live Server (Recommended)
```bash
# 1. Download index.html, style.css, README.md into one folder
# 2. Open folder in VS Code
# 3. Install "Live Server" extension by Ritwick Dey
# 4. Right-click index.html → Open with Live Server
# 5. Opens at: http://127.0.0.1:5500/index.html
```

### Option 2 — Direct Browser Open
```bash
# Just double-click index.html — it opens in your browser!
# (Dark/light mode toggle works, all animations work)
```

### Option 3 — Python Server
```bash
cd portfolio-folder
python -m http.server 8080
# Visit: http://localhost:8080
```

---

## 🌐 Live Demo

```
https://pranavvaidhya.github.io/pranav-portfolio
```

---

## 📁 File Structure

```
pranav-portfolio/
├── index.html     # Complete HTML structure (9 sections)
├── style.css      # Advanced CSS3 styling (600+ lines)
└── README.md      # This documentation file
```

---

## 🖼️ Screenshots

> Add screenshots after deployment

| Desktop Dark | Desktop Light | Mobile |
|---|---|---|
| `[screenshot-dark.png]` | `[screenshot-light.png]` | `[screenshot-mobile.png]` |

---

## 🎨 Design System

| Element | Value |
|---|---|
| Primary Font | Playfair Display (headings) |
| Body Font | Outfit (body text) |
| Dark Accent | `#c8f55a` (lime green) |
| Light Accent | `#5a8f00` (dark lime) |
| Border Radius | 10px / 18px / 28px / 40px |
| Transition | `0.3s cubic-bezier(0.4, 0, 0.2, 1)` |

---

## 📄 License

MIT — free to use and modify.

---

*Developed with ♥ by **Pranav Vaidhya** — Advanced CSS3 & Responsive Architecture*
