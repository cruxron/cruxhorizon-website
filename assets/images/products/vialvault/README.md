# VialVault product visuals

This directory is reserved for real VialVault product screenshots. Do not add
mock interfaces or placeholder images.

## Intended assets

- `hero.webp` — primary product view for the hero; recommended source export at
  least 1600 px wide
- `dashboard.webp` — dashboard or overview view
- `inventory.webp` — inventory capability
- `schedule.webp` — scheduling and reminders capability
- `details.webp` — record history or detail/logging capability

Use optimised WebP files where practical and retain an original source outside
the deployed website when needed.

## Adding the hero visual

In `products/vialvault/index.html`:

1. Remove `hidden`, `aria-hidden="true"`, and `data-asset-state="empty"` from
   the hero `.product-showcase` figure.
2. Add `has-product-visual` to `.product-hero-layout`.
3. Insert an image with intrinsic dimensions, for example:

   `<img class="asset-frame__media" src="../../assets/images/products/vialvault/hero.webp" width="1600" height="1000" alt="VialVault dashboard showing [describe the visible workflow]">`

Alt text must describe what the real screenshot communicates. Do not use a
generic value such as "VialVault screenshot".

## Adding capability visuals

The inventory, scheduling, and record-history cards each contain a hidden
`.capability-visual` figure:

1. Remove `hidden`, `aria-hidden="true"`, and `data-asset-state="empty"`.
2. Add `has-product-visual` to the parent `.capability-card`.
3. Insert the relevant image with `width`, `height`, and specific alt text.
4. Add a `<figcaption>` only when it provides useful context not already in the
   surrounding capability copy.

The prepared layout places an activated visual alongside its capability copy on
larger screens and stacks it below the copy on smaller screens.

## Presentation utilities

Reusable classes in `assets/css/site.css` are available when real assets arrive:

- `.asset-frame` — standard bordered screenshot frame
- `.asset-frame--device` — deeper device-style surround
- `.asset-frame--flush` — removes inner frame padding
- `.asset-frame__media` — responsive image sizing
- `.asset-caption` — optional explanatory caption

Add `data-asset-state="empty"` and `hidden` while a frame has no real image.
Empty frames are never displayed. Remove both only after inserting the asset.

Hero imagery should normally load eagerly. Below-the-fold capability screenshots
may use `loading="lazy"` and `decoding="async"`. Always include intrinsic `width`
and `height` to reduce layout movement.

Every screenshot that communicates product information needs specific alt text.
Decorative imagery may use `alt=""`, but it must not contain information that is
missing from the surrounding text.
