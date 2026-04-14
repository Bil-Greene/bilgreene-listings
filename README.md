# bilgreene-listings
Single-property listing microsites for bilgreene.com

## Structure
- `property-template-v1.html` — master template, source of truth
- `pages/` — one HTML file per listing, generated from the template
- `assets/` — local dev assets only (production assets on Cloudflare R2)
- `docs/` — project documentation

## Workflow
Listing data → Claude → Cursor → pages/[address-slug].html → Cloudflare Pages

## Local dev
npx serve .
