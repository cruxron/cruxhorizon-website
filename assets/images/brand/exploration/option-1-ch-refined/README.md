# Refined CH monogram candidate

This is an isolated refinement candidate. It is not referenced by the live Crux
Horizon website and does not replace the current production logo.

## Files

- `icon.svg` — recommended primary icon: white C, blue H, navy tile
- `icon-mono.svg` — reverse single-colour icon for dark backgrounds
- `horizontal.svg` — colour horizontal lockup for dark backgrounds
- `horizontal-mono.svg` — dark single-colour horizontal lockup for light backgrounds

## Design decisions

### Integrated letter construction

The C forms a calm, stable enclosure. The H sits inside the opening rather than
beside it, making the mark one compact silhouette. Its crossbar establishes the
horizon and connects the two letterforms optically.

### Direction without an arrow

The outer H stem rises into one angled shoulder. This adds forward movement
without introducing an arrowhead, chevron, orbit, or generic technology motif.

### Optical spacing

The inner H stem stops before the C terminals. The separation prevents the
monogram from closing into a G shape and preserves the C opening at small sizes.
The right stem is intentionally heavier than the inner stem to counterbalance
the visual mass of the C.

### Colour

- Navy tile: `#07111F`
- Primary accent blue: `#69B1FF`
- Light mark colour: `#F4F7FB`
- Dark monochrome: `#07111F`

The colour icon is the recommended avatar, app-icon, and profile-image version.
Use monochrome only when production constraints require one colour.

## Small-size testing

The colour icon was rasterised directly from SVG and reviewed at each required
size:

| Size | Result |
| --- | --- |
| 16 px | C opening and blue H remain present; use primarily as a browser-scale fallback |
| 32 px | Both letters remain distinguishable and the angled shoulder survives |
| 64 px | Strong favicon, app-list, and compact-header performance |
| 180 px | Clear for Google Workspace profiles and social avatars |
| 512 px | Balanced for app-icon and presentation use without revealing unnecessary detail |

Do not add outlines, shadows, gradients, or internal detail to compensate at
small sizes.

## Recommended production candidate

`icon.svg` is the recommended standalone candidate. It has the strongest
small-size recognition, preserves the existing navy/blue/white system, and is
specific to the Crux Horizon name while remaining independent of any one product.

`horizontal.svg` is the recommended dark-surface lockup for continued review.
Before final brand approval, compare its custom all-caps vector wordmark with an
outlined version of the approved Crux Horizon website wordmark at actual header
size. The icon geometry should remain unchanged during that typography check.

## Remaining concerns

- In single-colour use the integrated letters are less immediate than in the
  colour version; avoid using the monochrome icon below 24 px where possible.
- The angled shoulder must not become steeper or extend beyond the current tile
  safe area, or it begins to read as an arrow.
- Confirm trademark availability before adopting the mark as a long-term asset.
