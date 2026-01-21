⚓ The "Brain-Breaking" CSS Nav
A reconstruction of the iconic navigation design by Raul Druut, built entirely with modern CSS and zero JavaScript. This project explores the power of the new CSS Anchor Positioning API to create fluid, tethered micro-interactions.

📺 Watch the Build
I documented the reconstruction of this navigation in a high-energy build log. [Watch on YouTube: [ Recreating Raul Druut’s Navigation ⚓ | Build Log
https://youtu.be/2dfI5QpGE4M ]

🚀 Technical Highlights
This project was a deep dive into solving common layout challenges using bleeding-edge CSS features:

CSS Anchor Positioning: Utilizing anchor-name on navigation links to dynamically tether the hover and active bubbles.

Zero-JS Logic: Using position-anchor and inset: anchor() to handle element tracking without the overhead of getBoundingClientRect.

Stacking Contexts: Managing complex layering (the "Z-index Dragon") using isolation: isolate to keep text readable over moving gradients.

Aesthetic Gradients: Multi-layered linear-gradient and box-shadow: inset to mimic a premium, glassmorphism UI.

🛠️ How it Works
The core logic relies on defining an anchor for each link:

CSS

/* Assigning the anchor */
.nav-link.active {
  anchor-name: --active-link;
}

/* Positioning the bubble */
.bubble-active {
  position: absolute;
  position-anchor: --active-link;
  inset: anchor(--active-link);
  transition: all 0.3s ease-in-out;
}
📂 Setup
Clone the repo:

Bash

git clone https://github.com/[YourUsername]/[RepoName].git
Open index.html in any modern browser (Chrome 125+ or Edge 125+ recommended for Anchor Positioning support).

🤝 Credits
Original Design: Raul Druut

Inspiration: Syntax.fm

Built by: [@013_web3boy] — Full-Stack Developer | Web3 Explorer | Music Enthusiast

📜 License
This project is licensed under the MIT License - see the LICENSE file for details.
