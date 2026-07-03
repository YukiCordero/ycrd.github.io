# Logo Usage Guide

This guide explains the production logo and favicon system for the Yuki Cordero portfolio brand. The logo system supports a premium dark-navy, gold, and cream identity while remaining flexible for light documents, social profiles, and small favicon surfaces.

## Logo files

All production logo SVGs are stored in `assets/logos/`.

### `yc-logo-primary-light.svg`

Primary full logo for light backgrounds. Use this version on white, cream, pale gold, light gray, or other high-contrast light surfaces. It is best for proposals, profile PDFs, light website sections, document headers, and presentation title slides.

### `yc-logo-reversed-dark.svg`

Reversed full logo for dark backgrounds. Use this version on the portfolio header, dark navy hero sections, dark cards, social banners, and dark presentation slides. This is the active logo used in the current website header and footer.

### `yc-icon-standalone.svg`

Standalone YC monogram. Use this when the full wordmark would be too wide or when the brand needs a compact mark: avatars, social profile images, small badges, app-style icons, circular profile placements, watermarks, and compact UI surfaces.

### `yc-logo-monochrome.svg`

Single-color logo. Use this version when color reproduction is limited or when a restrained one-color mark is required: invoices, internal documents, low-color print, embossing, watermark use, or subtle footer applications. The file uses `currentColor`, so its final color can be controlled with CSS or the design tool.

## Favicon files

All production favicon files are stored in `assets/favicons/`.

- `yc-favicon.svg` — primary scalable favicon.
- `favicon-16x16.png` — small browser tab fallback.
- `favicon-32x32.png` — standard browser favicon fallback.
- `favicon-48x48.png` — larger desktop/browser fallback.
- `favicon-180x180.png` — high-resolution mobile fallback.
- `favicon-512x512.png` — large icon for manifest and high-density contexts.
- `apple-touch-icon.png` — iOS home-screen icon.
- `favicon.ico` — legacy browser fallback.

The website references the SVG favicon first, then `.ico` and PNG fallbacks, plus the Apple touch icon and web app manifest.

## Minimum display sizes

- Full logo lockup: minimum 180px wide on desktop and 150px wide on mobile.
- Standalone YC icon: minimum 32px wide in UI placements.
- Favicon: use the generated favicon files for 16px, 32px, and 48px contexts instead of scaling the full wordmark.
- Social/avatar icon: use at 180px or larger when possible to preserve the gold detail and premium feel.

## Clear-space rules

Use the height of the `Y` in the YC monogram as the clear-space unit. Keep at least 1x this unit around the standalone icon. For the full logo lockup, keep at least 0.75x this unit around the full mark. Do not let text, borders, photos, icons, or card edges enter this zone.

When the logo appears in a sticky header, leave enough vertical padding so the mark does not feel compressed. When the logo appears over a card or image, use a solid overlay or background panel to protect contrast.

## Background contrast guidance

- Use the reversed logo on dark navy, charcoal, black, deep blue, and dark gradient backgrounds.
- Use the primary light-background logo on cream, white, pale gray, and light gold backgrounds.
- Use the monochrome logo only when the final chosen color creates sufficient contrast against the background.
- Avoid placing the gold mark directly on busy photos, bright yellow/gold backgrounds, or low-contrast tan surfaces.
- Do not add drop shadows, strokes, bevels, or unapproved effects to compensate for weak contrast. Choose the correct logo version instead.

## Favicon usage guidance

Use the monogram favicon system for all browser, mobile, and manifest icons. Do not use the full horizontal wordmark as a favicon; it becomes unreadable at small sizes. The SVG favicon is preferred for modern browsers, while PNG and `.ico` files support older or platform-specific contexts.

## Production consistency

The supplied SVG logo files are path-based and do not rely on browser-rendered live text. If any logo is edited later in Figma, Illustrator, or Inkscape, convert all text to vector paths before exporting the final SVG files. This avoids browser font differences, spacing shifts, and wordmark weight changes.
