# Crux Horizon — reference CH energy refinement

This folder contains the final optical refinement of the approved `reference-ch-energy` exploration. It is isolated from the production brand assets and is not connected to the website.

## Changes made

- Increased the horizontal wordmark scale from `1.35` to `1.68` (24.4%) while retaining the existing vector-path letterforms.
- Re-centred the enlarged wordmark vertically in the 48-unit lockup and expanded the viewBox width to preserve clear artwork bounds.
- Reduced the diagonal's cross-width by approximately 8% without changing its centreline, direction, or endpoints.
- Lifted the H from `#247DE3` to `#2F86EB`. The energy line remains the brighter `#69B1FF`, preserving clear colour hierarchy.
- Preserved the original CH geometry, icon proportions, navy `#07111F`, white `#F4F7FB`, and flat-colour construction.

## Before and after

| Attribute | Reference | Refined | Result |
| --- | --- | --- | --- |
| Wordmark scale | 1.35 | 1.68 | 24.4% greater visible height |
| Wordmark height at 28px lockup | 9.45px | 11.76px | Stronger header authority |
| Wordmark height at 32px lockup | 10.8px | 13.44px | Better balance with the icon |
| Diagonal cross-width | 100% | 92% | Less dominance; clearer C/H read |
| H blue | `#247DE3` | `#2F86EB` | Better separation from navy |
| Energy blue | `#69B1FF` | `#69B1FF` | Signature highlight retained |

## Small-size review

- **16px favicon:** use `icon.svg`. The C, H, and rising diagonal remain distinct; the diagonal is intentionally close to a one-pixel visual weight at this size.
- **32px browser icon:** use `icon.svg`. The CH relationship reads clearly and the two blues remain separated.
- **28px and 32px website header:** use `horizontal.svg`. The enlarged wordmark is now visually authoritative without overtaking the icon anchor.
- **180px profile image:** use `icon.svg`; retain the complete square canvas and do not crop inside the rounded navy tile.
- **512px app icon:** use `icon.svg` as source artwork, applying platform-specific safe-area and corner-mask requirements during export.

The monochrome variants are intended for one-colour printing, embossing, engraving, and light-background documentation. Their current navy fill may be changed uniformly to the production medium's single ink colour; do not recolour individual components separately.

## Recommended production usage

`horizontal.svg` is the recommended website-header and business-document lockup on dark navy surfaces. `icon.svg` is the recommended source for favicons, browser icons, profiles, social avatars, and app-icon exports. The refined set should replace production artwork only after an in-context header review and explicit approval.

Keep clear space around either mark equal to at least one quarter of the icon height. Do not add gradients, shadows, glows, outlines, textures, or rearrange the C, H, and diagonal.

## Technical notes

All four SVGs use explicit vector paths, valid viewBoxes, flat fills, and accessible titles and descriptions. They contain no SVG text, external fonts, embedded raster images, gradients, filters, or external dependencies.
