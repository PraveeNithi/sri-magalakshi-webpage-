# Sri Mahalaxmi Hardware

A single-page website for **Sri Mahalaxmi Hardware** — a hardware shop at 102, Fort Main Road, Shevapet, Salem 636002. The site showcases the shop's product range (doors, door fittings and all hardware tools) and makes it one tap to call or message the shop.

## Features

- **Loading screen** — circle shop logo with the shop name, shown for ~3.6 s on page load.
- **Sticky masthead** — shop logo + name with an always-visible "Call now" button.
- **Photographic hero** — full-width shop photo with tagline and Call / WhatsApp buttons.
- **Product catalogue** — all product photos in a responsive grid (2 / 3 / 4 columns). Tap any photo to open a full-size lightbox.
- **Contact panel** — two call lines, WhatsApp, Instagram, email, Google Maps directions, and a share button.
- **Mobile sticky bar** — persistent Call / WhatsApp buttons at the bottom of the screen on phones.
- **Accessibility** — keyboard focus rings, alt text, reduced-motion support, no horizontal scroll.
- **SEO** — meta description and `HardwareStore` structured data (JSON-LD) for Google.

## Tech

- Plain HTML + CSS + a small amount of vanilla JS. No build step, no dependencies.
- Fonts: Fraunces (display) + Switzer (body) loaded from Google Fonts / Fontshare.
- Images live in `images/`.

## Running locally

The page is fully static — open `index.html` directly, or serve the folder:

```sh
# Python 3
python -m http.server 8080
```

Then open <http://localhost:8080>.

## Project structure

```
index.html      # entire site (markup, styles, scripts)
images/
  hero1.png     # hero photograph
  logo.png      # shop logo
  tool1.jpg…    # product photos (19 items)
README.md
```

## Deploying on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages** and set the source to the `main` branch.
3. Wait for the deploy, then open `https://<username>.github.io/sri-mahalaxmi-hardware-shop-/`.

> Note: the page references images under `images/`. Make sure those files are committed — GitHub Pages serves exactly what is in the repository.

## Contact details on the site

- Phone: 9600650607 · 6380246462
- WhatsApp: +91 9600650607 / +91 6380246462
- Instagram: @srimahalaxmihardwareslm
- Email: srimahalaxmi2025hardwareslm@gmail.com
- Address: 102, Fort Main Road, Shevapet, Salem — 636002

## Editing the content

All shop details (phone numbers, address, social links) live in `index.html`. Search for `tel:` / `wa.me` / `instagram.com` to update them in one place each.

To add or remove product photos, add the file to `images/`, then add/remove a `<figure class="tile">` block in the product grid inside `index.html`. The section text says how many items are listed — update it to match.
