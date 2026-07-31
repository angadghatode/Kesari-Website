# Kesari | Karta Farms Digital Presence

A bespoke, static website for Karta Farms — a regional flour milling and logistics business based in Hines Hill, Western Australia.

This project establishes the digital footprint for their premium wheat product line, **Kesari**, serving as the primary consumer touchpoint and supporting retail partnerships, including product availability at Spudshed locations across WA.

---

## 🎯 Business Goals

- Communicate Kesari's farm-to-table heritage and brand story
- Provide clear product information and storage guidelines
- Drive foot traffic to local retail partners (Spudshed)
- Offer a direct contact channel for B2B and B2C enquiries via Formspree

---

## 🛠️ Technical Stack

A two-page static site. No build step, no framework — intentionally lightweight for fast load times and easy deployment.

| Layer | Technology |
|---|---|
| Markup | HTML5 — semantic, accessible |
| Styling | Tailwind CSS (CDN, utility layout) + `styles.css` (design system, animations, masking) |
| Scripting | Vanilla JS — mobile nav toggle, FAQ accordion |
| Forms | [Formspree](https://formspree.io) — serverless email relay |
| Fonts | Google Fonts — Playfair Display (headings), Poppins (body) |
| Icons | Remix Icon (CDN) |

---

## 📁 Structure

```
Kesari-Website/
├── index.html          # Landing page — hero, journey, quality, FAQ, contact
├── about-us.html       # Brand story page — hero, contact
├── css/
│   └── styles.css      # Design system: tokens, components, responsive rules
├── assets/             # Photography, brand logo, hand-drawn illustrations
└── README.md
```

---

## 🎨 Design System

All design tokens live in `:root` inside `styles.css`:

- **Palette** — warm cream (`#FBF7F1`), tan, deep tan, ink brown, and an orange accent (`#D6862E`)
- **Navbar & Footer** — dark brown (`#2E1A0E`) for a consistent brand frame
- **Typography** — Playfair Display (serif headings) + Poppins (body)
- **Image blending** — `mix-blend-mode: multiply` on hand-drawn PNGs removes their white backgrounds naturally against warm cream sections. Logo badges in the navbar and footer use `isolation: isolate` to control the compositing context.

---

## 📐 Layout Highlights

- **Hero sections** — full-bleed photo absolutely positioned to the right (index) or left (about-us), masked with a CSS gradient fade. On mobile, photo stacks above text with a downward fade.
- **Journey section** — four-step grid (`steps-grid`) where each `.step-item` pairs its numbered badge with its arch-shaped photo card, keeping them aligned at every breakpoint.
- **Promise section** — image bleeds off the left edge with an organic curved border-radius.
- **FAQ + Find Us** — two-column layout with accordion FAQs on the left and a Spudshed retail card on the right. The windmill illustration decorates the bottom-right corner via `mix-blend-mode: multiply` on the white section background.

---

## 📱 Responsive

Single breakpoint at `900px`. At mobile:

- Hero and about-us images stack above text with a bottom-fade mask
- Journey steps collapse from 4-column to 2-column (numbers remain paired with their cards)
- Promise image becomes a standard rounded rectangle
- FAQ/Find Us stacks to single column; decorative illustrations hidden
- Navbar opens a full-screen dark overlay matching the header colour