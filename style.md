# Style Guide — calebsobo.com

## Typography

**Font:** Geist (variable, 100–900 weight)
Source: `geist` npm package, loaded via `@font-face` from `node_modules/geist/dist/fonts/geist-sans/Geist-Variable.woff2`

| Element | Size | Weight | Other |
|---|---|---|---|
| Eyebrow | 11px | 400 | Uppercase, 0.1em letter-spacing |
| H1 | 28px | 500 | Line-height 1.2 |
| Title | 15px | 400 | — |
| Blurb / body | 14px | 300 | Line-height 1.6 |
| Contact label | 11px | 400 | Uppercase, 0.08em letter-spacing |
| Contact value / links | 14px | 400 | — |
| Resume button | 12px | 400 | Uppercase, 0.06em letter-spacing |
| Copy hint | 11px | 400 | — |

---

## Colors

### Light mode

| Token | Hex | Usage |
|---|---|---|
| Background | `#ffffff` | Page background |
| Foreground | `#111111` | H1, links, buttons, borders |
| Title | `#555555` | Job title line |
| Blurb / note | `#777777` | Body copy, portfolio note |
| Eyebrow | `#999999` | "Portfolio — Under Construction" label |
| Contact label | `#bbbbbb` | "Email", "LinkedIn" labels |
| Copy hint | `#bbbbbb` | "copied" feedback text |
| Divider | `#e5e5e5` | Horizontal rule |

### Dark mode (`prefers-color-scheme: dark`)

| Token | Hex | Usage |
|---|---|---|
| Background | `#0f0f0f` | Page background |
| Foreground | `#ededed` | H1, links, buttons, borders |
| Title | `#aaaaaa` | Job title line |
| Blurb / note | `#999999` | Body copy, portfolio note |
| Eyebrow | `#888888` | "Portfolio — Under Construction" label |
| Contact label | `#666666` | "Email", "LinkedIn" labels |
| Copy hint | `#666666` | "copied" feedback text |
| Divider | `#222222` | Horizontal rule |

---

## Layout

- **Max content width:** 480px, centered horizontally and vertically
- **Page padding:** 48px top/bottom, 24px left/right
- **Content is vertically and horizontally centered** in the viewport via flexbox

---

## Spacing

| Element | Value |
|---|---|
| Eyebrow → H1 | 20px bottom margin |
| H1 → title | 6px bottom margin |
| Title → blurb | 12px bottom margin |
| Blurb → divider | 36px bottom margin |
| Divider → contact | 28px bottom margin |
| Contact item gap | 12px |
| Contact label width | 60px (fixed) |
| Resume button top | 28px |
| Resume buttons gap | 10px (inline margin) |

---

## Components

### Resume / CTA Button
- Border: 1px solid foreground color
- Padding: 8px 16px
- No background (transparent default)
- Hover: background fills to foreground color, text inverts
- Transition: background and color, 0.15s

### Email Copy Button
- Styled as plain text (no border, no background)
- Same font size and color as other contact values
- Hover: underline

### Links
- No underline by default
- Underline on hover
- Color matches foreground

### Divider
- `<hr>` with no border, only a 1px top border
- Color: `#e5e5e5` (light) / `#222222` (dark)
