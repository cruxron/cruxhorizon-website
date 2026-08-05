# Crux Horizon production brand assets

This directory contains the approved Crux Horizon `reference-ch-energy-refined`
production identity system. The artwork is built entirely from SVG paths and
uses no external fonts, raster images, gradients, filters, or dependencies.

## Production selection

The approved identity combines an angular CH monogram with a rising diagonal
energy element and a custom outlined wordmark. Do not rotate, rearrange,
redraw, or apply effects to these elements.

- `logo.svg` — primary horizontal colour lockup for dark Crux Horizon surfaces
- `logo-on-dark.svg` — explicit dark-background horizontal colour lockup
- `logo-on-light.svg` — approved single-colour horizontal lockup for white or
  pale surfaces
- `logo-mono.svg` — single-colour horizontal lockup for one-ink production
- `mark.svg` — compact colour CH icon on its navy tile
- `mark-mono.svg` — compact single-colour CH icon without a background tile
- `favicon.svg` — compact colour CH icon used by browser favicon references

The production files are promoted from
`exploration/reference-ch-energy-refined/`. That exploration directory remains
the approved source record; production pages reference only the files in this
directory.

## Approved colours

- Navy background: `#07111F`
- White: `#F4F7FB`
- CH blue: `#2F86EB`
- Energy and wordmark accent blue: `#69B1FF`

Do not introduce gradients, glow, shadows, textures, outlines, or additional
colours inside the logo artwork.

## Horizontal lockup usage

Use `logo.svg` or `logo-on-dark.svg` in website headers and on dark navy
surfaces. They contain the white C and “Crux” letterforms, blue H and “Horizon”
letterforms, and the brighter diagonal energy element.

Use `logo-on-light.svg` on white and pale neutral surfaces. It is intentionally
the approved navy monochrome lockup rather than an unapproved recoloured
variant. Use `logo-mono.svg` for one-colour printing, embossing, engraving, and
other restricted production methods. A print vendor may change every navy fill
uniformly to the selected single ink; individual components must not be
recoloured separately.

Maintain clear space equal to at least one quarter of the icon height. Do not
display the horizontal lockup below 120 px wide. The website currently renders
`logo-on-dark.svg` at a 28 px height through the shared `.brand-logo` rule.

## Icon usage

Use `mark.svg` for profiles, social avatars, app identity, and other compact
colour applications. Retain the complete square canvas and navy tile. Apply
platform-specific safe areas and corner masks only during exported app-icon
production; do not crop the source artwork.

Use `mark-mono.svg` for one-colour document and merchandise applications. Do
not place the navy monochrome mark on a dark background without changing the
entire mark uniformly to a suitable single light ink.

The minimum approved icon size is 16 px. Prefer 32 px or larger whenever space
allows.

## Favicon usage

`favicon.svg` is the approved colour CH icon and is active through the existing
root-relative favicon reference on every HTML page. Its 64 × 64 viewBox scales
cleanly to 16 px and 32 px browser sizes.

Do not add separate details to the favicon artwork. If raster favicon formats
are required later, export them directly from `favicon.svg` with the complete
navy tile intact.

## Accessibility

Horizontal logos used as the only visible content of a link require meaningful
alternative text such as `alt="Crux Horizon"`. Do not add duplicate visually
hidden brand text to the same link. Decorative duplicate marks should use an
empty `alt` attribute.

Each SVG includes an accessible title and description. Preserve these when
optimising or exporting the artwork.

## Remaining raster assets

- `apple-touch-icon.png` — future 180 × 180 px opaque PNG exported from
  `mark.svg`
- `social-preview.png` — future 1200 × 630 px Open Graph and social card image

Do not enable references to these files until the real production exports
exist. Keep essential social-preview content inside a central safe area.
