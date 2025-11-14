# FirmOS Marketing Site Clone

Pixel-accurate recreation of the FirmOS marketing experience. The page promotes an AI-powered operating system for accounting firms and mirrors the structure, interactions, and motion design of the original Webflow site.

## Overview
- **Single-page experience** focused on educating accounting-firm leaders about FirmOS and capturing waitlist signups.
- **Static export** built from Webflow markup, enhanced with lightweight custom CSS/JS tweaks for modals, sticky navigation, and responsive behaviour.
- **Third-party embeds** for analytics, trust signals, and media (YouTube, Trustpilot, Customer.io Forms, PostHog, Microsoft Clarity, Sentry).
- **CTA coverage** with “Join Waitlist” buttons, embedded forms, and direct links to the production app `app.firmos.ai`.

## Highlights
- **Hero + explainer video modal** introduces the “Smartest Way to Scale Your Accounting Firm” positioning with autoplay-ready YouTube embeds.
- **Feature pillars** (Business Development, Talent, Operations) open detailed modal cards describing AI automations such as lead scraping, AI career agent, SOP generator, and KPI dashboards.
- **Process & benefits sections** show step-by-step adoption, KPI lifts, and trust-building stats tailored for accounting firm operators.
- **Success stories carousel** aggregates testimonials and Trustpilot social proof to emphasize credibility.
- **FAQ accordions** answer implementation questions while reinforcing outcomes and service guarantees.
- **Responsive navigation** adapts between desktop menu, mobile drawer, and contextual CTA buttons to maintain conversion focus.

## Tech Stack
- HTML5 + semantic sections exported from Webflow.
- Compiled Webflow CSS plus small custom overrides inside `index.html`.
- Vanilla JavaScript for navbar toggles, feature modals, FAQ accordions, and embedded player controls.
- External services: Google Tag Manager, Google Analytics 4, PostHog, Microsoft Clarity, Sentry, Trustpilot widgets, Customer.io forms, Plerdy heatmaps, and Vector pixel.

## Getting Started
1. **Clone the repo**
   ```bash
   git clone https://github.com/<your-handle>/firmos-site.git
   cd firmos-site
   ```
2. **Serve locally**
   - Quick preview (Windows): `start index.html`
   - Cross-platform preview: `python -m http.server 8080` then open `http://localhost:8080`
3. **Deploy**
   - Upload the static files to any host (GitHub Pages, Netlify, Vercel static, S3/CloudFront, etc.).  
   - Ensure third-party env keys (PostHog, GTM, etc.) remain valid or replace them with your own.

## Customization Guide
- **Branding**: swap logos, colors, and copy directly in `index.html`. Global accents live near the top of the file inside `<style>` blocks.
- **Imagery**: replace CDN image URLs with local assets or your own CDN for long-term stability.
- **Data tracking**: update the IDs for GA4, GTM, PostHog, Clarity, and Trustpilot to avoid sending data to FirmOS accounts.
- **Forms & CTAs**: edit the `Join Waitlist` links/customer.io embed configs to point at your mailing list or CRM.
- **Performance**: consider inlining critical CSS, self-hosting fonts, or pruning unused Webflow scripts if you plan to productionize the clone.

## Credits & Attribution
This project is a pixel-perfect educational clone of [firmos.ai](https://www.firmos.ai). All product names, copy, and visuals remain the property of their respective owners and are used here for learning/demo purposes only.

## License
No explicit open-source license has been applied. Add a license (e.g., MIT, Apache-2.0) before distributing or adapting the work publicly.

