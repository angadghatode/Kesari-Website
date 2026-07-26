# Kesari | Karta Farms Digital Presence

A bespoke, static website developed for Karta Farms, a regional flour milling and logistics business based in Hines Hill, Western Australia. 

This project establishes the digital footprint for their premium wheat product line, **Kesari**, serving as a primary touchpoint for customers and supporting regional retail partnerships, including product availability at Spudshed locations across WA.

## 🎯 Business Impact & Project Scope
Moving a traditional agricultural and milling operation into the digital space requires a focus on brand authenticity and accessibility. The goal was to build a lightweight, high-fidelity landing page that:
*   Communicates the farm-to-table heritage of the Kesari brand.
*   Provides clear product information and storage guidelines to consumers.
*   Drives foot traffic to local retail partners.
*   Offers a direct communication channel for B2B and B2C inquiries.

## 🛠️ Technical Architecture
To prioritize speed, maintainability, and deployment simplicity for a two-page architecture, the project intentionally avoids heavy JavaScript frameworks in favor of a clean, vanilla stack. 

*   **HTML5:** Semantic markup ensuring accessibility and clear document structure.
*   **CSS3 & Tailwind CSS:** A hybrid approach using Tailwind via CDN for rapid structural utility classes, paired with a custom `styles.css` file to handle complex UI elements (like CSS masking, custom typography, and `mix-blend-mode` asset integration).
*   **Vanilla JavaScript:** Lightweight DOM manipulation for mobile navigation and interactive FAQ accordions, keeping the bundle size negligible.

## 📁 Repository Structure
The project strictly adheres to a separation of concerns, keeping styling, markup, and assets cleanly organized:

```text
karta-farms-web/
├── index.html           # Main landing page and brand overview
├── about-us.html        # Detailed heritage and milling process
├── css/
│   └── styles.css       # Custom styling, animations, and design system variables
├── assets/              # Optimized imagery, SVG iconography, and brand assets
└── README.md