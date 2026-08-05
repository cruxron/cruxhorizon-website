# Reference-led CH energy exploration

This folder is an isolated logo exploration based on the supplied reference
image. It is not referenced by the live Crux Horizon website.

## Files

- `icon.svg` — primary white, blue, and navy icon
- `icon-mono.svg` — dark single-colour icon for light surfaces
- `horizontal.svg` — colour icon and vector-path wordmark for dark surfaces
- `horizontal-mono.svg` — dark single-colour lockup for light surfaces

## Design decisions

### CH construction

The C is a wide angular enclosure with a deliberately open right side. The H is
reduced to a strong right stem and horizontal shoulder. The diagonal energy line
completes the relationship between the letters rather than adding a fourth
decorative element.

### Diagonal energy line

The reference image's rising blue diagonal is retained as the distinctive part
of the identity. It is rebuilt as a constant-width parallelogram rather than a
glowing or tapered stroke. At 16 px it remains approximately 1.5 px thick, which
keeps it visible without relying on effects.

### Flat production geometry

The artwork contains no gradients, shadows, glow, textures, clipping masks, or
raster content. All visible elements are filled paths with hard edges and a
small number of anchor points.

### Colour

- Navy background: `#07111F`
- White C: `#F4F7FB`
- Blue H: `#247DE3`
- Energy blue: `#69B1FF`
- Dark monochrome: `#07111F`

## Scale testing

The primary icon was rasterised directly from SVG and reviewed at 16, 32, 64,
180, and 512 px.

- **16 px:** the diagonal, white C, and blue H remain separated; the diagonal is
  the first-read feature.
- **32 px:** the CH structure becomes clear and the line retains a crisp edge.
- **64 px:** suitable for browser UI, compact navigation, and app lists.
- **180 px:** strong for Google Workspace profiles and social avatars.
- **512 px:** balanced for app-icon and business presentation use.

## Comparison with the previous CH refinement

Compared with `../option-1-ch-refined/`:

- This version is closer to the supplied reference and preserves its diagonal
  identity cue.
- The previous version is calmer and more conventional, with a more literal H.
- This version has a stronger silhouette and greater distinctiveness in profile
  and app-icon contexts.
- The diagonal dominates more at 16 px, while the previous mark prioritises the
  letterforms first.
- This version separates C and H spatially, reducing the earlier risk of the
  integrated monogram reading as G/H in monochrome.

## Recommendation

Use `icon.svg` as the preferred candidate for reference-led evaluation. It is
more memorable than the previous CH exploration and better preserves continuity
with the supplied identity direction.

Before production adoption, test the icon in real browser tabs on both standard
and high-density displays. If the diagonal feels too dominant at 16 px, create a
favicon-specific optical variant by reducing its width by no more than 10%; do
not remove it or add effects.
