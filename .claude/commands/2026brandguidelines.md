# Casa 2026 Brand & Design System

When designing or building UI for any project, apply the following design system exactly unless told otherwise. This captures all fonts, colors, spacing, component patterns, and visual language used to build Casa applications.

---

## Typography

### Font Families
- **Primary / UI:** `'Maison Neue', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`
  - Weight 400 → MaisonNeue-Book.otf
  - Weight 600 → MaisonNeueWEB-Demi.woff / MaisonNeue-Demi.otf
- **Serif / Editorial:** `'CMU Serif', Georgia, serif`
  - Used for: card titles, stat labels, tab bar, modal labels, section subheadings, user name in header
  - Conveys authority and warmth alongside the sans-serif UI

### Type Scale
| Role | Size | Weight | Color | Notes |
|------|------|--------|-------|-------|
| App name | 19px | 700 | white | header |
| Brand subtitle | 15px | 400 | `rgba(255,255,255,0.5)` | CMU Serif, 0.2px tracking |
| Main tab label | 15.5px | 400 | `#6b7280` active → `#6d20da` | CMU Serif |
| Subtab label | 13.5px | 400 | `#6b7280` active → `#6d20da` | Maison Neue |
| Card title | 16px | 400 | `#140919` | CMU Serif, 0.2px tracking |
| Section label (uppercase) | 10.5–11px | 600 | `#9ca3af` | uppercase, 0.7–0.9px tracking |
| Body / form | 14px | 400 | `#111827` | |
| Label | 12.5px | 500 | `#374151` | |
| Hint / meta | 11–11.5px | 400 | `#9ca3af` | |
| Stat value | 22px | 700 | `#111827` | -0.5px tracking |
| Large stat value | 30px | 700 | role-dependent | compa gauge |
| Results title | 18px | 700 | `#111827` | -0.3px tracking |
| Table header | 11px | 600 | `#6b7280` | uppercase, 0.06em tracking |
| Table cell | 13–13.5px | 400 | `#111827` | |
| Badge / chip | 10.5–11.5px | 600 | role-dependent | |

---

## Color Palette

### Brand
| Token | Hex | Usage |
|-------|-----|-------|
| **Navy (darkest)** | `#12122a` | App header background, offer letter header/footer, logo background |
| **Purple primary** | `#6d20da` | Active tabs, focus rings, toggle on-state, midpoint line, primary gradient start |
| **Purple light** | `#818cf8` | Gradient end, avatar background |
| **Purple muted** | `#5046e5` | Employee name chip in results, generate-offer button |
| **Purple faint** | `#ede9fe` | HR role badge bg, band fill gradient start, level chip P-track bg |
| **Purple softer** | `#ddd6fe` | Band fill gradient end, increase box secondary bg |
| **Purple whisper** | `#faf8ff` | Active tab background |
| **Taupe dark** | `#5c4f45` | Admin role badge text, midpoint value labels, M/E/CXO chip text, summary bar accent |
| **Taupe light** | `#e4d9ce` | Admin role badge bg, M/E/CXO level chip bg |

### Semantic
| Token | Hex | Usage |
|-------|-----|-------|
| **Green success** | `#16a34a` | In-band offer dot/line, stat highlight border-bottom, approve action |
| **Green bg** | `#dcfce7` | Highlight stat box, rec box green, increase box |
| **Green mid** | `#bbf7d0` | Gradient end for green boxes |
| **Green border** | `#86efac` | Highlight stat border |
| **Green deep** | `#166534` | Approved status badge text |
| **Amber warning** | `#d97706` | Edited/dragged offer dot, warning stat border-bottom |
| **Amber bg** | `#fef9c3` | Warning stat box, pending approval badge |
| **Amber mid** | `#fde68a` | Warning gradient end |
| **Red danger** | `#dc2626` | Out-of-band indicator, danger stat border-bottom, error states |
| **Red bg** | `#fee2e2` | Danger stat box, login error |
| **Red mid** | `#fecaca` | Danger gradient end |
| **Blue info** | `#1d4ed8` | Partial approval badge text |
| **Blue info bg** | `#dbeafe` | Partial approval badge bg |
| **Sky accent** | `#0ea5e9` | Header gradient (3rd stop) |
| **Teal accent** | `#10b981` | Header gradient (4th stop), active-session dot |

### Neutral
| Token | Hex | Usage |
|-------|-----|-------|
| **Text primary** | `#111827` | All primary text |
| **Text secondary** | `#374151` | Labels, rec text, body copy |
| **Text muted** | `#6b7280` | Inactive tabs, subtitles, table muted |
| **Text faint** | `#9ca3af` | Hints, sub-labels, section headers |
| **Border default** | `#e4e7ef` | Inputs, cards, dividers |
| **Border light** | `#e5e7eb` | Table row separators |
| **Border faintest** | `#f3f4f6` | Row hover, faint separators |
| **Surface 0** | `white` | Cards, modals, inputs |
| **Surface 1** | `#f9fafb` | Table headers, disabled inputs, secondary surfaces |
| **Surface 2** | `#f8f9fc` | Stat boxes, notes area |
| **Surface 3** | `#f0f2f8` | App background, band track, type toggle bg, lookup track |
| **Surface 4** | `#ecedf2` | Hover tint on tabs and subtabs |
| **Overlay** | `rgba(0,0,0,0.35)` | Modal backdrop |

### Role Badges
| Role | Background | Text |
|------|-----------|------|
| Administrator | `#e4d9ce` | `#5c4f45` |
| HR | `#ede9fe` | `#5b21b6` |
| Approver | `#d6eadf` | `#1e5c3a` |
| Finance (custom) | `#f5d9e8` | `#8b3361` |

### Level Chips
| Track | Prefix | Background | Text |
|-------|--------|-----------|------|
| Individual Contributor | P | `#ede9fe` | `#6d20da` |
| Manager | M | `#e4d9ce` | `#5c4f45` |
| Executive | E / CXO | `#e4d9ce` | `#5c4f45` |
| Fallback | — | `#f3f4f6` | `#6b7280` |

---

## Gradients

| Name | Value | Used on |
|------|-------|---------|
| Header accent bar | `linear-gradient(90deg, #6d20da, #818cf8, #0ea5e9, #10b981)` | 3px top stripe, offer letter accent |
| Logo mark / avatar | `linear-gradient(135deg, #6d20da, #818cf8)` | App logo, user avatar |
| Primary button | `linear-gradient(135deg, #1a1a2e 0%, #2d2d50 100%)` | Generate button |
| Active type toggle | `linear-gradient(135deg, #6d20da, #a855f7)` | Selected offer type pill |
| Band fill | `linear-gradient(90deg, #ddd6fe, #a5b4fc)` | Salary band visualization |
| Download button | `linear-gradient(135deg, #6d20da, #818cf8)` | PDF download |
| Green stat | `linear-gradient(135deg, #dcfce7, #bbf7d0)` | In-band stat boxes |
| Amber stat | `linear-gradient(135deg, #fef9c3, #fde68a)` | Warning stat boxes |
| Red stat | `linear-gradient(135deg, #fee2e2, #fecaca)` | Danger stat boxes |

---

## Spacing & Sizing

| Token | Value |
|-------|-------|
| Page max-width | `1280px` |
| Page padding | `28px 24px` |
| Card padding | `26px 28px` |
| Card gap | `20px` |
| Form field gap | `16px` |
| Form label gap | `5px` |
| Button padding (primary) | `13px` full-width |
| Button padding (secondary) | `13px 18px` |
| Input padding | `10px 14px` |
| Stat box padding | `14px 16px` |
| Table cell padding | `12–13px 14px` |
| Modal padding | `28px 32px` |

---

## Border Radius

| Element | Radius |
|---------|--------|
| Cards | `16px` |
| Modals | `16–20px` |
| Inputs, selects, textareas | `10px` |
| Buttons (primary, reset) | `10px` |
| Buttons (small/action) | `6–8px` |
| Badges / pills | `20px` |
| Level chips | `10px` |
| Stat boxes, rec boxes | `12px` |
| Band track | `12px` |
| Type toggle container | `10px`, pills inside `8px` |
| Logo mark | `9px` |
| Avatar | `50%` (circle) |
| Tag-style badges | `20px` |

---

## Shadows & Borders

| Element | Shadow / Border |
|---------|----------------|
| Card | `0 1px 3px rgba(0,0,0,0.05), 0 0 0 1px rgba(0,0,0,0.04)` |
| Login card | `0 4px 24px rgba(0,0,0,0.08), 0 0 0 1px rgba(0,0,0,0.04)` |
| Modal | `0 20px 60px rgba(0,0,0,0.18)` |
| Offer letter | `0 24px 64px rgba(0,0,0,0.22)` |
| Active type toggle | `0 2px 8px rgba(109,32,218,0.35)` |
| Offer dot (in-band) | `0 2px 8px rgba(22,163,74,0.4)` |
| Input focus ring | `0 0 0 3px rgba(109,32,218,0.1)` |
| Stat box (highlight) | `border-bottom: 3px solid #16a34a` |
| Stat box (warning) | `border-bottom: 3px solid #d97706` |
| Stat box (danger) | `border-bottom: 3px solid #dc2626` |
| Tab active underline | `border-bottom: 4px solid #6d20da` |
| Default input border | `1.5px solid #e4e7ef` |

---

## Component Patterns

### Cards
White background, `16px` radius, subtle shadow + 1px ring. Title in CMU Serif 16px/400. Padding `26px 28px`.

### Buttons — Primary (Generate)
Full-width, navy gradient (`#1a1a2e → #2d2d50`), white text 14.5px/600, `10px` radius, `13px` vertical padding. Hover: `opacity 0.88`. Active: `scale(0.99)`.

### Buttons — Secondary (Reset / Print)
White bg, `1.5px solid #e4e7ef`, `#6b7280` text. Hover: `#f9fafb` bg, `#d1d5db` border.

### Buttons — Small Table Actions
`5px 12px`, `6px` radius, `12px/500`, white bg, default border. Variants: `--danger` (red), `--approve` (green), `--letter` (purple).

### Type Toggle
Full-width pill group on `#f0f2f8` bg. Inactive pill: `#e4e6ef`. Active pill: purple gradient + `0.35` shadow. Smooth 0.18s transition.

### Inputs & Selects
`1.5px solid #e4e7ef`, `10px` radius, `10px 14px` padding, 14px text. Focus: purple border + 3px focus ring. Disabled: `#f9fafb` bg.

### Stat Boxes
`#f8f9fc` bg, `12px` radius, transparent border. Label in CMU Serif 16px/400. Value 22px/700. Sub 11px muted. Colored variants get gradient bg + colored bottom border.

### Badges / Pills
`border-radius: 20px`, 10.5–11.5px/600. Color pairs: see Role Badges and Level Chips tables above.

### Band Visualization
Gray track (`#f0f2f8`, `12px` radius, `44px` tall). Purple gradient fill. Purple `2px` midpoint line with upward triangle. Green dot (18px, 3px white border, 8px grab shadow) + green line for offer. Yellow when dragged, gray when out-of-band.

### Tables
Header: `11px` uppercase/600, `#6b7280`, `#f9fafb` bg, `1px #e5e7eb` bottom border. Cells: `12–13px 14px` padding, `1px #f3f4f6` bottom. Row hover: `#fafafa`. `white-space: nowrap` on all `td`.

### Tabs (Main)
CMU Serif, 15.5px/400, `#6b7280`. Hover: `#ecedf2` bg. Active: `#6d20da` text + 4px purple bottom border + `#faf8ff` bg.

### Subtabs
Maison Neue, 13.5px/400, same hover/active logic as main tabs. Subtab bar on `#f9fafb` bg with `1px #e4e7ef` bottom.

### Modals
White, `16px` radius, large shadow, max-width 560px (confirm: 380px). Header with title + close (gray pill button). Grid layout for detail fields.

### Role Editor Toggle (Permission Switches)
Custom toggle: 40×22px pill, `#e5e7eb` off, `#6d20da` on. White 16px thumb slides 18px on check.

---

## Motion

| Property | Value |
|----------|-------|
| Default transition | `0.15s ease` |
| Tab color/border | `0.15s` |
| Input border/shadow | `0.15s` |
| Type toggle | `0.18s` |
| Button hover opacity | `0.15s` |
| Offer dot/line position | `0.05s` (drag tracking) |
| Toggle thumb | `0.2s` |
| Scale on active button | `scale(0.99)` |

---

## Header Pattern
Dark navy (`#12122a`) bar. 3px rainbow gradient accent strip above it. Logo mark: purple gradient 34×34 `9px` radius box with bold initials. App name 19px/700 white. Subtitle in CMU Serif, muted white. Right cluster: session badge (glass pill) + user card (glass pill with avatar + name + logout).

## Page Background
`#f0f2f8` — cool blue-gray, not pure gray.

## Iconography
Emoji icons used sparingly for status (✓ ⚠ ↑ ↓). No icon library — SVG chevrons inline in CSS for select dropdowns.

## Empty States
Centered column: 52×52 `14px`-radius icon box (`#f0f2f8`), 16px/600 title, 13.5px muted description, max-width 320px.
