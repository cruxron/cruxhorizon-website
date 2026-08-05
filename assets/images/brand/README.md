# Crux Horizon production brand assets

This directory contains only the active Crux Horizon brand assets used by the
production website.

## Active assets

- `logo-on-dark.svg` — horizontal Crux Horizon logo used in all website headers
- `favicon.svg` — square Crux Horizon browser icon used by all HTML pages

The current artwork is approved production artwork. Do not redraw, optimise,
simplify, recolour, or otherwise modify either SVG without explicit approval.

## Website references

Root pages reference the header logo as:

`assets/images/brand/logo-on-dark.svg`

Pages under `products/vialvault/` reference it as:

`../../assets/images/brand/logo-on-dark.svg`

All pages reference the favicon with the root-relative path:

`/assets/images/brand/favicon.svg`

## Accessibility

Header logo images use `alt="Crux Horizon"` because they are the only visible
content of their homepage links. Avoid adding duplicate hidden brand text to
the same links.
