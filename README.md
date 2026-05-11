A personal design system built from the ground up for my UX portfolio. It documents the visual language, component patterns, and design decisions used consistently across my portfolio site and case studies.

---

## Overview

This design system was created to bring consistency and intentionality to my portfolio work. Rather than making ad-hoc design decisions page by page, I extracted and formalized the patterns that were already emerging across my projects — color usage, typography pairing, component behavior, and spacing — into a single referenceable system.

The token file is formatted for direct import into **Tokens Studio for Figma**, making it ready for design handoff and future development.

---

## What's Included

| File | Description |
|------|-------------|
| `faustina-design-tokens.json` | Full design token set importable into Tokens Studio for Figma |
| `README.md` | This file |

---

## Design Tokens Structure

Tokens are organized into three layers:

### `global`
Raw, primitive values. These are the source of truth.
- **Color** — brand yellows, interactive blues, creative pinks, professional lavenders, and neutrals
- **Typography** — font families, sizes, weights, line heights, letter spacing
- **Spacing** — 6-step scale from 4px to 80px
- **Border radius** — 4 variants from tags (4px) to avatars (full)
- **Border width** — thin to featured

### `semantic`
Named roles that reference global tokens. This is the layer applied to Figma elements.
- `text.primary`, `text.secondary`, `text.interactive`, `text.on-dark`
- `background.page`, `background.footer`, `background.card-professional`, `background.card-creative`
- `border.default`, `border.accent-blue`, `border.accent-yellow`
- `highlight.teaching`, `highlight.motion`, `highlight.photography`

### `components`
Token sets scoped to specific UI components.
- **Nav** — link states, font size, active color
- **Button** — 4 variants: primary, secondary, CTA (yellow), link
- **Card** — background, border, radius, padding
- **Footer** — background, text colors, font size
- **Highlight Label** — Playground page section labels
- **Info Card** — CoStar-style paired content cards

---

## Color Palette

| Token | Hex | Usage |
|-------|-----|-------|
| `brand.yellow` | `#F5D98B` | Logo accent, footer, CTAs |
| `brand.yellow-dark` | `#E8C050` | Borders on brand elements |
| `brand.yellow-footer` | `#FAE9A0` | Footer background across all pages |
| `interactive.blue` | `#3B6BC4` | Active nav, links, professional card footers |
| `interactive.blue-light` | `#6B9DE8` | Hover states |
| `accent.pink` | `#F4A7C3` | Creative project accents (TuneFuse) |
| `accent.pink-light` | `#FADADF` | Creative case study section backgrounds |
| `accent.lavender` | `#A8A0D8` | Professional project accents (CoStar) |
| `accent.lavender-light` | `#D4CFFB` | Professional case study section backgrounds |
| `neutral.black` | `#111111` | Primary text, dark backgrounds |
| `neutral.surface` | `#F7F6F2` | Component and section backgrounds |

---

## Typography

| Role | Font | Weight | Size |
|------|------|--------|------|
| Display / Name | Playfair Display | 700 | 36–40px |
| Tagline (italic) | Playfair Display | 400 italic | 16px |
| H1 Page heading | DM Sans | 700 | 28–32px |
| H2 Section heading | DM Sans | 700 | 20–22px |
| H3 Card title | DM Sans | 700 | 15–16px |
| Body | DM Sans | 400 | 14–16px |
| Nav / Label | DM Sans | 500 | 11–12px |
| Caption | DM Sans | 400 | 10–11px |

---

## Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `xs` | 4px | Icon gaps, tight padding |
| `sm` | 8px | Inner component gaps |
| `md` | 16px | Card padding, nav gaps |
| `lg` | 24px | Section internal spacing, grid gutters |
| `xl` | 48px | Between page sections |
| `2xl` | 80px | Hero and major section breaks |

---

## How to Import into Figma

1. Install the [Tokens Studio for Figma](https://tokens.studio/) plugin (free)
2. Open the plugin inside your Figma file
3. Go to **Settings → Load from file / URL**
4. Select `faustina-design-tokens.json`
5. Tokens will appear in three groups: `global`, `semantic`, and `components`
6. Apply semantic tokens to your Figma frames and components — if you ever update a global value, all elements using that token update automatically

---

## Design Decisions

**Why two accent colors?**
Pink (creative/warm) and lavender (professional/cool) are used intentionally to signal the nature of each project at a glance. TuneFuse and motion work use pink; CoStar and structured UX work use lavender. They never appear on the same section.

**Why Playfair Display + DM Sans?**
Playfair adds personality and warmth to the name/tagline — it reflects the human, emotional side of the brand. DM Sans is clean and legible at small sizes without feeling cold, making it ideal for body copy and UI labels.

**Why yellow as the brand anchor?**
Yellow appears in the footer on every single page of the portfolio. It creates a consistent visual bookend that ties all content together regardless of which case study is being viewed.

---

## About

**Faustina Koduah** is a UX Designer and Motion Graphics specialist based in Virginia, currently studying Business Information Systems at Virginia Commonwealth University. Previous Product Design Intern at CoStar Group.

[Portfolio](https://faustina.design) · [LinkedIn](https://linkedin.com/in/faustinakoduah)

---

*Design system documented and tokenized in 2026.*
