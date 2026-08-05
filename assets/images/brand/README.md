# Crux Horizon brand assets

This directory is reserved for final, production-approved Crux Horizon brand
assets. Do not add temporary artwork or generated placeholders.

## Required files

- `favicon.svg` — square SVG browser icon, recommended `viewBox="0 0 32 32"`;
  designed to remain clear at 16 × 16 px and 32 × 32 px
- `apple-touch-icon.png` — 180 × 180 px PNG for Apple home-screen bookmarks;
  opaque background recommended
- `social-preview.png` — 1200 × 630 px PNG for Open Graph and social cards;
  keep essential content inside a central safe area
- `logo.svg` — primary scalable Crux Horizon logo or wordmark; use a tight
  horizontal `viewBox` appropriate to the artwork (approximately 5:1 for a
  wordmark), and avoid embedded raster images or external font dependencies

## Activation

The HTML files contain inactive, root-relative metadata hooks for the favicon,
Apple touch icon, and social preview. Enable those tags only after the matching
production files exist at the paths above.

### Logo

Every current `.brand` link contains an inactive example for `logo.svg`. After
the production logo has been added:

1. Replace the visible `Crux <span>Horizon</span>` text inside each `.brand`
   link with the documented `<img>` element.
2. Keep `alt="Crux Horizon"` so the linked logo retains its accessible name.
3. Keep the root-relative `/assets/images/brand/logo.svg` path on all pages.
4. Verify the artwork at the shared `.brand-logo` display height of 28 px and
   at narrow mobile widths.

Do not keep both meaningful image alt text and visually hidden duplicate brand
text, because that can create a repeated accessible name. If a future layout
keeps visible text beside the mark, use `alt=""` on the decorative image and
leave the text as the accessible label.

### Browser icons

After both icon files exist, uncomment the prepared `<link rel="icon">` and
`<link rel="apple-touch-icon">` elements in every page head. Confirm that the
SVG favicon has no external resources and that the PNG is exactly 180 × 180 px.

### Social preview

When `social-preview.png` is added, enable both `og:image` and `twitter:image`,
then change `twitter:card` from `summary` to `summary_large_image` on every page.
Use `https://cruxhorizon.com/assets/images/brand/social-preview.png` as the
absolute social image URL.

If `logo.svg` is displayed in page content, provide an accessible name through
descriptive `alt` text on `<img>` or `aria-label` on a linked logo. A purely
decorative duplicate mark should use `alt=""` and must not carry information
that is unavailable in text.
