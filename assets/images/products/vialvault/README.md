# VialVault product visuals

This directory is reserved for real VialVault product screenshots. Do not add
mock interfaces or placeholder images.

## Intended assets

- `hero-product-screenshot.webp` — primary product view for the hero
- `dashboard-screenshot.webp` — dashboard or overview view
- `inventory-screenshot.webp` — inventory capability
- `scheduling-screenshot.webp` — scheduling and reminders capability
- `detail-logging-screenshot.webp` — record history or detail/logging capability

Use optimised WebP files where practical and retain an original source outside
the deployed website when needed.

## Adding the hero visual

In `products/vialvault/index.html`:

1. Remove `hidden`, `aria-hidden="true"`, and `data-visual-state="empty"` from
   the hero `.product-showcase` figure.
2. Add `has-product-visual` to `.product-hero-layout`.
3. Insert an image with intrinsic dimensions, for example:

   `<img src="../../assets/images/products/vialvault/hero-product-screenshot.webp" width="1600" height="1000" alt="VialVault dashboard showing [describe the visible workflow]">`

Alt text must describe what the real screenshot communicates. Do not use a
generic value such as "VialVault screenshot".

## Adding capability visuals

The inventory, scheduling, and record-history cards each contain a hidden
`.capability-visual` figure:

1. Remove `hidden`, `aria-hidden="true"`, and `data-visual-state="empty"`.
2. Add `has-product-visual` to the parent `.capability-card`.
3. Insert the relevant image with `width`, `height`, and specific alt text.
4. Add a `<figcaption>` only when it provides useful context not already in the
   surrounding capability copy.

The prepared layout places an activated visual alongside its capability copy on
larger screens and stacks it below the copy on smaller screens.
