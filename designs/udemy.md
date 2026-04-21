# Udemy — Design Language

## Aesthetic

Marketplace-first, accessible, and value-driven. Udemy's design prioritizes discoverability and purchase conversion across a massive catalog of 200,000+ courses. The purple brand anchors a clean white-dominated layout. Typography is compact and readable for dense catalog browsing. Constant pricing signals (sale badges, original vs. discounted price) and social proof (star ratings, learner counts) are integral design elements, not add-ons.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand Purple | `#A435F0` | Primary CTAs, links, active indicators |
| Brand Dark | `#7719AA` | Button hover, pressed states |
| Brand Light | `#F4E9FF` | Selected states, highlights |
| Link Purple | `#5624D0` | Inline links, breadcrumbs |
| Background | `#FFFFFF` | Page, card surfaces |
| Background Secondary | `#F7F9FA` | Section fills, sidebar |
| Background Dark | `#1C1D1F` | Footer, dark hero |
| Text Primary | `#1C1D1F` | All headings, body copy |
| Text Secondary | `#6A6F73` | Meta, descriptions, captions |
| Text Link | `#5624D0` | Inline text links |
| Text on Dark | `#FFFFFF` | Text on dark surfaces |
| Border | `#D1D7DC` | Card edges, inputs, dividers |
| Success | `#1D6B2A` | Completion, enrolled badge |
| Warning | `#F5922E` | Limited-time sale alerts |
| Error | `#D9534F` | Form errors |
| Rating Star | `#E59819` | Course rating stars |
| Bestseller Badge | `#E59819` | Bestseller label background |

## Typography

**Font:** Udemy Sans (fallback: SF Pro Text, system-ui) — a humanist sans-serif optimized for compact reading in catalog contexts.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Hero heading | 35px | 700 | 1.2 |
| Page heading | 28px | 700 | 1.2 |
| Section heading | 23px | 700 | 1.2 |
| Card title | 16px | 700 | 1.4 |
| Body | 16px | 400 | 1.4 |
| Small body | 14px | 400 | 1.4 |
| Caption / meta | 12px | 400 | 1.4 |

## Spacing

Base unit: 4px.

| Token | Value | Usage |
|-------|-------|-------|
| 2xs | 4px | Badge padding, tight gaps |
| xs | 8px | Icon-text gaps, tag padding |
| sm | 12px | List item spacing |
| md | 16px | Card internal padding |
| lg | 24px | Component gaps |
| xl | 32px | Section spacing |
| 2xl | 48px | Page section padding |
| 3xl | 64px | Large section separators |

## Layout

- Max content width: 1340px
- 12-column grid, 16px gutters (tighter than most — maximizes catalog density)
- Course catalog: 4-col cards (desktop), 3-col (medium), 2-col (small), 1-col (mobile)
- Sticky header: 64px with search bar prominent
- Course page: 65% content / 35% sticky enrollment sidebar
- Checkout: 2-column order summary layout

## Components

**Buttons**
- Primary: `#A435F0` fill, white text, 4px radius, 700 weight
- Secondary: white fill, `#1C1D1F` border and text
- Black CTA: `#1C1D1F` fill, white text (used in cart/checkout)
- Height: 48px (large), 40px (default)
- Hover: brand-dark `#7719AA`

**Course Cards**
- White bg, 4px radius, thin border on hover only (no default border)
- Top: thumbnail image (16:9)
- Title (700, 16px, 2-line clamp), instructor name (14px, secondary), star rating (gold `#E59819` stars + score + count), price with strikethrough original
- Bestseller badge: `#E59819` bg, black text, 0px radius (rectangular tag feel)
- Hover: shadow appears `0 4px 8px rgba(0,0,0,0.12)`, course preview video starts

**Price Display**
- Discounted price: bold, large (`#1C1D1F`)
- Original price: smaller, strikethrough, `#6A6F73`
- Discount %: `#E59819` or red badge

**Star Rating**
- Gold filled/half/empty stars (12px)
- Numeric score bold beside stars
- Learner count in secondary text + "(X ratings)"

**Inputs**
- 1px `#D1D7DC` border, 4px radius, 8px 12px padding
- Focus: 2px `#A435F0` border
- Search input: prominent, 48px height, magnifier icon

**Course Progress Bar**
- `#A435F0` fill on `#F7F9FA` track, 8px height

## Visual Patterns

- Sale countdown banner at top of page (black bg, white text, orange discount)
- Category breadcrumbs at top of all course pages
- "What you'll learn" — checklist section with `#1C1D1F` checkmarks
- Instructor profile section with avatar, bio, rating, review count
- Course curriculum accordion — expandable sections with lesson counts and durations
- "Students also bought" horizontal scroll of course cards
- Certificate of completion preview illustration
- Refund policy badge ("30-Day Money-Back Guarantee")

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 100ms | Button hover, star fill |
| Duration base | 200ms | Card hover shadow, dropdown |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | All transitions |

Course card preview video fades in on hover (200ms delay). Shadow appears on card hover. Minimal animation — conversion-focused UX avoids anything that delays click-to-purchase flow.
