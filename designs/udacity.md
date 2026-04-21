# Udacity — Design Language

## Aesthetic

Tech-forward, dark, and career-focused. Udacity targets professional developers and engineers, reflecting this in a bold dark-mode-first palette with electric cyan and deep navy. The visual language signals industry credibility — partnerships with companies like Google, AWS, and Mercedes-Benz are prominent. Typography is geometric and assertive. The feel is more bootcamp than university.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand Cyan | `#02B3E4` | Primary actions, links, highlights, progress |
| Brand Dark | `#0189B0` | Hover states |
| Brand Light | `#E0F7FD` | Light-mode highlights |
| Accent Red | `#FF5555` | Error states, urgency, discount badges |
| Background | `#FFFFFF` | Light mode pages |
| Background Secondary | `#F4F4F4` | Section fills |
| Background Dark | `#1A1A2E` | Dark hero, dark sections |
| Background Dark Secondary | `#16213E` | Card surfaces in dark sections |
| Text Primary | `#1A1A2E` | Body text (light mode) |
| Text Secondary | `#5C5C6E` | Meta, captions |
| Text on Dark | `#FFFFFF` | All text on dark backgrounds |
| Border | `#E0E0E0` | Inputs, card edges |
| Success | `#00A651` | Completion, passing grade |
| Warning | `#FFC107` | Near-deadline notices |
| Error | `#FF5555` | Validation failures |

## Typography

**Font:** Montserrat — geometric, confident. Heavy weights for hero text convey ambition and momentum.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Hero heading | 48px | 800 | 1.2 |
| Section heading | 36px | 700 | 1.2 |
| Card title | 24px | 600 | 1.4 |
| Body | 16px | 400 | 1.6 |
| Caption / meta | 14px | 400 | 1.6 |
| Label | 12px | 600 | 1.3 |

Letter spacing: +0.05em on uppercase labels and button text.

## Spacing

Base unit: 8px.

| Token | Value | Usage |
|-------|-------|-------|
| xs | 8px | Icon gaps, badge padding |
| sm | 16px | Card internal padding |
| md | 24px | Component spacing |
| lg | 32px | Section header gaps |
| xl | 48px | Section padding |
| 2xl | 64px | Large section vertical spacing |
| 3xl | 96px | Hero section padding |

## Layout

- Max content width: 1280px, centered
- 12-column grid, 32px gutters
- Nanodegree catalog: 3-col cards (desktop), 2-col (tablet)
- Dark hero section full-width with centered text
- Company partner logos in horizontal scrolling strip
- Learning path: vertical timeline layout in course detail

## Components

**Buttons**
- Primary: `#02B3E4` fill, white text, 8px radius, 800 weight, uppercase, 0.05em letter spacing
- Secondary: transparent bg, `#02B3E4` border and text
- CTA size: 52px height, 24px 48px padding
- Hover: brightness 110%, subtle scale 1.02

**Nanodegree Cards**
- Dark bg `#16213E` in hero sections, white bg in catalog
- Top: program image or video thumbnail
- Content: Nanodegree name (700), duration, difficulty, monthly price
- Partner company logos (Google, AWS etc.) displayed at bottom
- "Enroll Now" button — full-width, brand cyan

**Project Showcase Cards**
- Student project examples with screenshot preview
- Graduate name + job title after completing program
- Company they joined post-graduation (social proof)

**Progress Tracker**
- Left sidebar in lesson view: project checklist
- `#02B3E4` filled circles for completed lessons
- Connecting vertical line between checkpoints

**Inputs**
- Dark mode: `#1A1A2E` bg, `#02B3E4` focus border
- Light mode: white bg, `#E0E0E0` default border

## Visual Patterns

- Company partnership logos prominent on hero — Google, AT&T, GitHub, AWS
- "Career Services" section with outcomes data (salary, hiring rate)
- Dark gradient hero overlaid on abstract tech imagery
- Certification badge illustrations (shield shape) on completion
- "Industry Expert" instructor profiles with company affiliation
- "Free Preview" video thumbnails with play overlay
- Project submission showcase — real student work examples

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 150ms | Button hover, focus states |
| Duration base | 300ms | Card hover, modal open |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | All transitions |

Cards slightly scale up (1.02) on hover. Smooth shadow elevation change. Progress bars animate on load with easing.
