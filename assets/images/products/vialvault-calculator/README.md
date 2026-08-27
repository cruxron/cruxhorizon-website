# VialVault Calculator product visuals

This directory is reserved for real VialVault Calculator product screenshots.
Do not add mock interfaces or placeholder images.

## Intended assets

- `hero.webp` — primary Calculator view for the hero; recommended source export
  at least 1600 px wide
- `reconstitution.webp` — reconstitution / vial amount workflow
- `draw-volume.webp` — intended amount to draw volume result
- `syringe.webp` — U-100 syringe visualisation

Use optimised WebP files where practical and retain an original source outside
the deployed website when needed.

## Adding the hero visual

In `products/vialvault-calculator/index.html`:

1. Remove `hidden`, `aria-hidden="true"`, and `data-asset-state="empty"` from
   the hero `.product-showcase` figure.
2. Add `has-product-visual` to `.product-hero-layout`.
3. Insert an image with intrinsic dimensions, for example:

   `<img class="asset-frame__media" src="../../assets/images/products/vialvault-calculator/hero.webp" width="1600" height="1000" alt="VialVault Calculator showing [describe the visible workflow]">`

Alt text must describe what the real screenshot communicates. Do not use a
generic value such as "VialVault Calculator screenshot".

## Adding capability visuals

Prepared capability cards may contain a hidden `.capability-visual` figure:

1. Remove `hidden`, `aria-hidden="true"`, and `data-asset-state="empty"`.
2. Add `has-product-visual` to the parent `.capability-card`.
3. Insert the relevant image with `width`, `height`, and specific alt text.

## Presentation utilities

Reusable classes in `assets/css/site.css` are available when real assets arrive:

- `.asset-frame` — standard bordered screenshot frame
- `.asset-frame--device` — deeper device-style surround
- `.asset-frame__media` — responsive image sizing

Add `data-asset-state="empty"` and `hidden` while a frame has no real image.
Empty frames are never displayed.
