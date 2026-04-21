# Coursera — Design Language

## Aesthetic

Clean, academic, and trustworthy. Coursera pairs a deep cobalt blue with generous white space to convey institutional credibility. Typography blends a serif heading face with readable sans-serif body text, evoking a university setting translated to digital. The overall tone is professional and approachable — serious education made accessible.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand | `#0056D2` | Primary buttons, links, active nav, progress bars |
| Brand Dark | `#003BA3` | Button hover, focus rings |
| Brand Light | `#E8F0FD` | Selected states, info banners, highlight backgrounds |
| Background | `#FFFFFF` | Page background, card surfaces |
| Background Secondary | `#F5F7FA` | Section fills, sidebar, footer |
| Background Dark | `#1F1F1F` | Dark nav bar, footer |
| Text Primary | `#1F1F1F` | Body copy, headings |
| Text Secondary | `#636363` | Metadata, captions, labels |
| Text Disabled | `#AEAEAE` | Inactive states |
| Border | `#D9D9D9` | Card borders, dividers, inputs |
| Success | `#008800` | Completion, correct answer |
| Warning | `#F5A623` | Deadlines, alerts |
| Error | `#E00000` | Form errors, critical states |
| Rating Star | `#F5A623` | Course star ratings |

## Typography

**Heading font:** Source Serif Pro — adds academic gravitas to course titles and hero text.  
**Body font:** Source Sans Pro — legible and neutral for dense course description copy.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Hero heading | 42px | 700 | 1.3 |
| Section heading | 32px | 700 | 1.3 |
| Card title | 24px | 600 | 1.4 |
| Body | 16px | 400 | 1.6 |
| Caption / meta | 14px | 400 | 1.6 |
| Badge / label | 12px | 600 | 1.3 |

Letter spacing: normal for body, +0.5px for uppercase labels and badges.

## Spacing

Base unit: 4px. Component padding follows an 8px grid.

| Token | Value | Usage |
|-------|-------|-------|
| 2xs | 4px | Icon gaps, tight inline spacing |
| xs | 8px | Chip padding, icon-text gap |
| sm | 12px | List item padding |
| md | 16px | Card inner padding, form field spacing |
| lg | 24px | Card gap, section sub-padding |
| xl | 32px | Section header spacing |
| 2xl | 48px | Section vertical padding |
| 3xl | 64px | Hero padding, major section gaps |
| 4xl | 96px | Top-of-page hero section |

## Layout

- Max content width: 1440px; main container max 1200px
- 12-column grid, 24px gutters
- Course catalog: 4-col card grid (desktop), 2-col (tablet), 1-col (mobile)
- Sticky top nav at 64px height
- Sidebar layout for course pages: 68% content / 32% info panel

## Components

**Buttons**
- Primary: `#0056D2` fill, white text, 8px radius, 16px 24px padding, 600 weight
- Secondary: white fill, `#0056D2` border, `#0056D2` text
- Hover: brand-dark `#003BA3`
- Height: 48px (large), 40px (default), 32px (small)

**Course Cards**
- White bg, 1px `#D9D9D9` border, 8px radius
- Top: course thumbnail image (16:9 ratio)
- Content area: title (600), provider logo + name, star rating, enrollment count, price
- Hover: shadow lifts to `0 4px 16px rgba(0,0,0,0.16)`
- Partner logo strip at bottom

**Inputs**
- 1px `#D9D9D9` border, 4px radius, 16px padding
- Focus: 2px `#0056D2` border, no shadow
- Error: `#E00000` border + message below

**Progress Bar**
- `#0056D2` fill on `#E8F0FD` track, 4px height, pill radius

**Breadcrumb / Nav**
- `#0056D2` links, `#636363` separator

## Visual Patterns

- University partner logos displayed prominently with consistent sizing
- Certificate preview cards with gold accents
- "Skills you'll gain" tag clouds — pill badges with `#E8F0FD` bg, `#0056D2` text
- Instructor headshots: circular crop, 64px
- Progress rings for course completion tracking
- Enrollment counts with human-readable formatting ("1.2M enrolled")
- Professional certificate banners with gradient overlay on dark bg

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 150ms | Button states, focus rings |
| Duration base | 250ms | Card hover, dropdown, accordion |
| Duration slow | 400ms | Page transitions, progress updates |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | All transitions |

Subtle shadow lift on card hover. Smooth progress bar fill animation. No decorative or distracting motion.
