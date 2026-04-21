# edX — Design Language

## Aesthetic

Bold, institutional, and globally minded. edX uses a deep crimson brand against white and dark navy to evoke the prestige of MIT and Harvard where it was founded. The design is structured and content-dense, prioritizing navigation clarity for learners exploring a large catalog. Clean sans-serif typography with high contrast conveys academic rigor without formality.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand | `#C00000` | Primary CTA buttons, active links, highlights |
| Brand Dark | `#8B0000` | Button hover, active states |
| Brand Light | `#FDECEA` | Info banners, selected states |
| Accent Navy | `#00262B` | Dark sections, footer, hero backgrounds |
| Background | `#FFFFFF` | Page and card backgrounds |
| Background Secondary | `#F7F7F7` | Section fills, sidebar |
| Background Dark | `#00262B` | Footer, dark hero, nav |
| Text Primary | `#000000` | Headings, body copy |
| Text Secondary | `#6C757D` | Meta text, descriptions, captions |
| Text on Dark | `#FFFFFF` | Text over dark/navy backgrounds |
| Border | `#DEE2E6` | Cards, inputs, dividers |
| Success | `#00873C` | Completion badges, correct answers |
| Warning | `#F0AD00` | Expiry notices, alerts |
| Error | `#C00000` | Form validation, errors |
| Info | `#0077C8` | Informational banners |

## Typography

**Font:** Inter — modern, highly legible neutral sans-serif. Consistent weight across all text levels.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Hero heading | 48px | 700 | 1.25 |
| Page heading | 32px | 700 | 1.25 |
| Section heading | 24px | 600 | 1.3 |
| Card title | 20px | 600 | 1.4 |
| Body | 16px | 400 | 1.5 |
| Caption / meta | 14px | 400 | 1.5 |
| Label / badge | 12px | 500 | 1.25 |

## Spacing

Base unit: 8px.

| Token | Value | Usage |
|-------|-------|-------|
| xs | 8px | Chip padding, tight gaps |
| sm | 12px | List item spacing |
| md | 16px | Card padding, input spacing |
| lg | 24px | Component gaps |
| xl | 32px | Section header gap |
| 2xl | 48px | Section padding |
| 3xl | 64px | Hero padding |
| 4xl | 96px | Top-level section spacing |

## Layout

- Max content width: 1200px, centered
- 12-column grid, 24px gutters
- Course catalog: 3-col grid (desktop), 2-col (tablet), 1-col (mobile)
- Sticky header at 64px
- Course detail: main content left, enrollment sidebar right (70/30 split)
- Dark footer with 4-column link grid

## Components

**Buttons**
- Primary: `#C00000` fill, white text, 4px radius, 12px 24px padding, 600 weight
- Enroll CTA: full-width in sidebar, large 48px height
- Secondary: white fill, `#000` border
- Hover: brand-dark `#8B0000`
- Rounded corners kept minimal (4px) — professional, not playful

**Course Cards**
- White bg, light `#DEE2E6` border, 4px radius
- Subject color band at top (category indicator)
- Title (600), institution name + logo, difficulty badge, duration
- Verified/Audit enrollment options shown as tabs within card

**Institution Badges**
- Logo + university name pairing, consistent 40px logo height
- Horizontal list in hero sections showing partner schools

**Inputs**
- 1px `#DEE2E6` border, 4px radius, 12px 16px padding
- Focus: 2px `#C00000` border
- Error: `#C00000` border and message

**Progress Indicator**
- Horizontal step bar for course progress
- `#C00000` completed, `#00873C` passed, `#DEE2E6` remaining

## Visual Patterns

- Hero with dark navy background and bold white typography
- MicroMasters and Professional Certificate program banners with gradient overlays
- Subject category icons with colored backgrounds
- "Audit for free" / "Verified" toggle — clear pricing transparency
- Learner outcome stats ("85% of learners see career benefit") in highlighted callout boxes
- Partner university logos in grayscale strip on white bg
- Video thumbnails with play button overlay

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 100ms | Button states |
| Duration base | 200ms | Card hover, dropdown |
| Duration slow | 350ms | Page transitions |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | All transitions |

Minimal animation — functional, not decorative. Card shadow lifts on hover. Smooth accordion expand for course syllabus sections.
