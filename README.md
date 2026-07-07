# Carlton Aesthetics — Website

Marketing website for **Carlton Aesthetics**, a pharmacist-led facial aesthetics clinic based within an established community pharmacy. The site's primary job is lead generation: visitors learn about treatments, have their safety questions answered, and get in touch via WhatsApp, phone, or the consultation form.

## Overview

- **Single-page static site** — no build step, no framework, no dependencies. One `carlton-aesthetics.html` file with embedded CSS and vanilla JS.
- **Brand-driven design** — porcelain cream and charcoal ink taken from the logo, wordmark recreated as live text in Cormorant Garamond, and the logo's flanked-rule device reused as the section-label system across the page. Body type is Jost; both faces load from Google Fonts.
- **Mobile-first** — the main audience arrives from Instagram, so navigation, contact cards, and CTAs are designed for tap targets first.
- **Accessible by default** — semantic landmarks, visible keyboard focus, native `<details>` FAQ, and `prefers-reduced-motion` respected for all scroll animations.

## Sections

Hero → credential strip (GPhC registration, insurance, clinical setting, licensed products) → treatments (anti-wrinkle, dermal fillers, aesthetics for men) → clinical standards → visit journey → about → FAQ → contact + enquiry form.

The "Our Standards" section deliberately answers the questions clients ask before choosing an injector: practitioner qualifications, insurance, hygiene, and product sourcing.

## Compliance note

Anti-wrinkle injections are prescription-only medicines in the UK. All copy avoids advertising POMs directly and describes treatment as *prescribed following a face-to-face consultation*, in line with ASA/MHRA advertising guidance. Keep this wording in mind when editing content.

## Running locally

Open the file in a browser — that's it.

```bash
open carlton-aesthetics.html        # macOS
# or
npx serve .                         # any OS, serves on localhost
```

## Before launch

- [ ] Replace the placeholder phone/WhatsApp number (`440000000000`) in the hero, contact cards, and `tel:`/`wa.me` links
- [ ] Add the pharmacy name and full address in the contact section
- [ ] Update the Instagram handle and link
- [ ] Add practitioner portrait photography (placeholder panel in the About section)
- [ ] Wire the enquiry form to an email service or WhatsApp Business API (currently front-end only)
- [ ] Add privacy policy, terms, and complaints procedure pages linked from the footer
- [ ] Set the production domain in `<meta>` tags and add analytics if required

## Deploying

Any static host works: GitHub Pages, Netlify, Vercel, Cloudflare Pages. For GitHub Pages, rename the file to `index.html`, push to `main`, and enable Pages in the repo settings.

---

© Carlton Aesthetics. All treatments delivered by a GPhC-registered pharmacist.
