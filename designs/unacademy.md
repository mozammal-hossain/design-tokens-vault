# Unacademy — Design Language

## Aesthetic

Minimalist, premium, and focused. Unacademy uses a near-black dark-first palette with an electric green accent — unusual for an edtech brand and highly distinctive. The design language is stripped back: heavy white space (or dark space), bold sans-serif typography, and very little decorative detail. The tone is serious and aspirational, targeting competitive exam candidates (UPSC, JEE, NEET) who need focus. A secondary light theme mirrors the same minimal system.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand Green | `#08BD80` | Primary buttons, active states, success, highlights |
| Brand Dark | `#06915F` | Hover, pressed states |
| Brand Light | `#E6FAF4` | Light-mode selected states |
| Background (dark) | `#080808` | Primary dark mode background |
| Background Secondary (dark) | `#141414` | Cards, panels on dark |
| Background Tertiary (dark) | `#1F1F1F` | Elevated surfaces on dark |
| Background (light) | `#FFFFFF` | Primary light mode background |
| Background Secondary (light) | `#F5F5F5` | Section fills on light |
| Text Primary (dark) | `#FFFFFF` | All text on dark bg |
| Text Secondary (dark) | `#A3A3A3` | Meta, captions, subtext |
| Text Primary (light) | `#080808` | All text on light bg |
| Text Secondary (light) | `#666666` | Captions, secondary info |
| Border (dark) | `#2B2B2B` | Card edges, dividers on dark |
| Border (light) | `#E0E0E0` | Card edges on light |
| Success | `#08BD80` | Correct, completed |
| Error | `#F44336` | Wrong, error states |
| Warning | `#FF9800` | Alerts, warnings |

## Typography

**Font:** Gilroy (fallback: Inter) — geometric, confident, modern. Heavy weights for display. The font choice signals a tech-premium brand positioning.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Hero / display | 48px | 800 | 1.2 |
| Section heading | 32px | 700 | 1.2 |
| Card title | 24px | 600 | 1.3 |
| Subheading | 18px | 600 | 1.4 |
| Body | 16px | 400 | 1.5 |
| Caption / meta | 14px | 400 | 1.5 |
| Label | 12px | 500 | 1.3 |

## Spacing

Base unit: 8px.

| Token | Value | Usage |
|-------|-------|-------|
| xs | 8px | Chip padding, icon gaps |
| sm | 12px | List item padding |
| md | 16px | Card padding, input spacing |
| lg | 24px | Component spacing |
| xl | 32px | Section header gaps |
| 2xl | 48px | Section padding |
| 3xl | 64px | Major section gaps |
| 4xl | 96px | Hero padding |

## Layout

- Max content width: 1280px
- Full-bleed dark hero sections
- Content grid: 12-column, 24px gutters
- Course catalog: 3-col (desktop), 2-col (tablet), 1-col (mobile)
- Live class: split layout — video left (70%), chat/sidebar right (30%)
- Educator profile: full-width banner + content below

## Components

**Buttons**
- Primary: `#08BD80` fill, white text, 8px radius, 600 weight, 48px height
- Secondary (dark): `#1F1F1F` fill, `#2B2B2B` border, white text
- Ghost: transparent bg, `#08BD80` border and text
- Hover: brand-dark `#06915F`

**Course Cards (dark mode)**
- `#141414` background, `#2B2B2B` border, 16px radius
- Top: thumbnail (16:9) with category badge
- Content: title (600, white), educator name, subject tag, price
- Live indicator: green dot + "LIVE" label when in session
- Hover: border brightens, subtle lift shadow

**Live Class Badge**
- Pulsing green dot + "LIVE" text in `#08BD80`
- Applied to cards and navigation items during live sessions

**Educator Cards**
- Circular educator photo (96px), name, subject, follower count
- Dark card surface, subtle border
- "Follow" pill button — outlined style

**Inputs**
- Dark mode: `#1F1F1F` bg, `#2B2B2B` border, white text
- Focus: `#08BD80` border
- Search bar: prominent, pill shape, top of page

**Tags / Badges**
- Exam category badges: pill shape, `#1F1F1F` bg, `#A3A3A3` text
- Active/selected: `#08BD80` bg, white text

## Visual Patterns

- Dark-first design — the primary experience is dark mode
- Full-bleed black hero sections with bold centered white typography
- Educator photo collages in hero — real faces build trust
- Exam name prominently labeled (UPSC, IIT-JEE, NEET, CAT)
- "Pro" subscription badge in gold on premium courses
- Live session viewer count displayed ("12,450 watching")
- Leaderboard / ranking tables for competitive exam prep
- Study plan timelines — vertical step layout

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 150ms | Button states, focus |
| Duration base | 250ms | Card hover, transitions |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | All transitions |

Pulsing animation on LIVE badge (opacity 1 → 0.4 → 1, 1.5s loop). Smooth card hover border highlight. Minimal motion overall — the focus-driven UX intentionally avoids distraction.
