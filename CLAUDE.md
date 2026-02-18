# RotiTales — Brand & Style Guide

## Color Palette (CSS custom properties only)

Never hardcode hex/rgb values in stylesheets. Always use the CSS custom properties defined in `:root` of `assets/css/style.scss`:

| Token              | Value     | Usage                              |
|--------------------|-----------|------------------------------------|
| `--flour`          | #FFF5E8   | Primary background                 |
| `--flour-light`    | #FFFDFA   | Lighter background variant         |
| `--flour-30`       | #FFF5E84D | 30% opacity flour                  |
| `--clay`           | #AB4F2E   | Primary accent / body text color   |
| `--clay-light`     | #CF9880   | Lighter clay                       |
| `--clay-30`        | #AB4F2E4D | 30% opacity clay                   |
| `--wheat`          | #F6BA59   | Secondary accent / highlights      |
| `--wheat-light`    | #FDE1B9   | Lighter wheat                      |
| `--wheat-30`       | #F5B8594D | 30% opacity wheat                  |
| `--warmth`         | #4D000A   | Deep red / headings                |
| `--warmth-dark`    | #240203   | Darkest brand shade / page bg      |
| `--warmth-30`      | #4D000A4D | 30% opacity warmth                 |
| `--abundance`      | #2E6121   | Green accent                       |
| `--abundance-light`| #98B690   | Lighter green                      |
| `--abundance-30`   | #2E61214D | 30% opacity green                  |

If you need a new shade, add a CSS custom property to `:root` — do not inline a hex value.

## Typography

- **Font**: `'Kufam', sans-serif` — the only font used across the site.
- There is no `--font-display` or other font variable. Always write `font-family: 'Kufam', sans-serif;` directly.

## Key Rules

1. **No hardcoded hex/rgb colors** outside `:root`. Use `var(--token)` everywhere.
2. **Stick to the brand palette.** Do not invent colors. If a new shade is needed, add it to `:root` with a descriptive name following the existing pattern (base / light / 30).
3. **z-index layers** (from low to high): carousel content (6) → tagline (7) → controls (10) → Follow button mobile (50) → nav & dropdowns (100) → cookie overlay (9999) → platform popup (10000).
4. **Mobile overrides** use the `.mobile-device` class (set via JS UA sniff on `<body>`), not media queries.
