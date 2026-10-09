# Roses Rockin' Childcare

Lightweight static childcare website with inline styles and JavaScript, system fonts, and an optimized local portrait. No build step or runtime dependencies.

## Files

- `public/index.html`: complete page, accessible mobile navigation, native FAQ, and business configuration.
- `public/image_0.svg`: supplied optimized portrait; keep with the HTML when publishing.

## Business details

Booking: https://calendar.app.google/YC3X1cnabWH8SSYv5

Edit `BUSINESS` in `public/index.html` and keep the static HTML fallbacks synchronized. Rates are currently unpublished and displayed as “Ask about current rates.” Only publish owner-approved prices, credentials, policies, and testimonials.

## Cloudflare Pages deployment

Project: `roses-rockin-childcare`

Production URL: https://roses-rockin-childcare.pages.dev/

Run from this repository with Node.js and Cloudflare authentication:

```sh
npx wrangler login
npx wrangler pages deploy public --project-name roses-rockin-childcare --branch main
```

Only deploy `public`, not the repository or home directory. For Git integration, use no framework, no build command, and `public` as the output directory. A GitHub push does not itself enable automatic Pages deployment.

## Verification

The September 2026 local design checks covered widths from 320 to 1440 CSS pixels, menu keyboard interaction, the skip link, FAQ disclosure, and the booking destination. Local Lighthouse results were desktop 100/100/100/100 and mobile 97/100/100/100 (Performance/Accessibility/Best Practices/SEO). These are historical local measurements, not guarantees for the deployed site or a complete WCAG audit.
