Urban Threads – Static E-commerce Website
=========================================
This repository contains a complete, single-page style e-commerce website for a modern clothing brand named Urban Threads. The site is designed to be mobile-responsive, visually striking, and playful with subtle micro-interactions while maintaining a clean, monochrome aesthetic with electric blue CTAs.

What’s included
- Home (index.html): Hero section with full-bleed image, New Arrivals, Best Sellers, and Testimonials. Long-form brand storytelling content.
- Shop (shop.html): 6 product cards with Add to Cart buttons. All prices are in INR (₹). Cart interactions persist in localStorage.
- Cart (cart.html): Fully functional cart page showing items, quantities, per-item totals, and a running cart total. Users can adjust quantity and remove items.
- Checkout (checkout.html): Simple checkout with an order summary, form fields, and a PayPal Sandbox mock payment flow. The total is calculated from the cart.
- About (about.html): Company story and philosophy.
- Contact (contact.html): Contact form with basic validation and Hyderabad address placeholder.
- README.md: This file, with setup and run instructions.

Tech notes and conventions
- All styling is done with Tailwind CSS utility classes via the CDN (no external CSS files needed for this demo).
- All images use placeholder syntax: src='https://pixabay.com/get/g67965bb23122a0ebcd4a30ee4cdca94e4d7e53447a6c9e871ce1e808c30d9f5b64a8a800cfc0af38b9e2d5b226a0f39c236ae051684fbeeb4a3ff21ecfaf5f62_640.jpg' to be replaced by server-side image processors.
- Fonts are loaded via a placeholder class on the HTML tag: class='{{font: Font Name}}'. The server should replace this placeholder with proper @font-face or a Google Font import.
- Currency is INR (₹) as requested.

How to run locally
1. Open the HTML files directly in a browser, or serve via a static server (e.g., npx serve in a Node environment).
2. Navigate between pages using the header navigation; on small screens, use the hamburger menu.
3. Interact with the Shop: add items to cart; the cart persists in localStorage.
4. Go to Cart to adjust quantities or remove items. Click Checkout to simulate a PayPal sandbox payment.

Notes
- The content is designed to be realistic with 500+ words per page where applicable.
- All interactive features (cart, checkout, modal, and mobile navigation) are implemented in JavaScript and rely on DOM events to function without server-side components.
- This is a static mockup intended for demonstration and design exploration. To transform into a production-ready site, integrate with a real backend, payment gateway, and proper accessibility improvements.