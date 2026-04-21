# BYJU'S — Design Language

## Aesthetic

Vibrant, aspirational, and parent-facing. BYJU'S design serves two audiences simultaneously: children (who use the app) and parents (who pay for it). The result is a professional, confidence-inspiring interface with energetic purple-navy gradients, friendly illustrations, and prominent achievement signals. Typography is rounded and approachable. Gradients — particularly the brand navy-to-purple — are the dominant visual motif, giving sections a premium and modern feel.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand Navy | `#1C2B5E` | Primary brand color, dark sections, headings |
| Brand Purple | `#6C3BAA` | Secondary brand, gradients, accents |
| Brand Gradient | `#1C2B5E → #6C3BAA` | Hero sections, CTA buttons, banners |
| Brand Light | `#E8EBF5` | Light bg for highlight sections |
| Accent Yellow | `#FFC107` | Achievement badges, CTAs, highlights |
| Background | `#FFFFFF` | Page surfaces, card backgrounds |
| Background Secondary | `#F5F6FA` | Section fills, sidebar |
| Background Dark | `#1C2B5E` | Header, footer, dark hero |
| Text Primary | `#1C2B5E` | All headings and body copy |
| Text Secondary | `#666D80` | Meta, captions |
| Text on Dark | `#FFFFFF` | Text over dark/gradient bg |
| Border | `#E2E5EE` | Cards, inputs, dividers |
| Success | `#00A651` | Correct answers, completed lessons |
| Warning | `#FFC107` | Streaks, reminders |
| Error | `#E53935` | Wrong answers, errors |

## Typography

**Font:** Nunito — friendly, rounded sans-serif. Balances approachability with readability across ages. Extra-bold weights for display headings convey confidence.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Hero / display | 56px | 800 | 1.2 |
| Section heading | 42px | 700 | 1.2 |
| Card heading | 24px | 600 | 1.3 |
| Subheading | 18px | 600 | 1.4 |
| Body | 16px | 400 | 1.6 |
| Caption / meta | 14px | 400 | 1.6 |
| Label / badge | 12px | 600 | 1.3 |

## Spacing

Base unit: 8px. Generous spacing — interface feels premium and uncluttered.

| Token | Value | Usage |
|-------|-------|-------|
| xs | 8px | Badge padding, tight gaps |
| sm | 16px | Card internal padding |
| md | 24px | Component spacing |
| lg | 32px | Section header gaps |
| xl | 48px | Section vertical padding |
| 2xl | 64px | Major section separators |
| 3xl | 80px | Page section padding |
| 4xl | 120px | Hero section top/bottom |

## Layout

- Max content width: 1200px
- Full-bleed gradient hero sections
- 12-column grid, 24px gutters
- Course catalog: 3-col grid (desktop), 2-col (tablet), 1-col (mobile)
- Homepage: large hero → stats strip → subject cards → testimonials → CTA
- In-app lesson: video centered, chapter list sidebar

## Components

**Buttons**
- Primary: gradient (`#1C2B5E → #6C3BAA`) fill, white text, 8px radius, 700 weight, 52px height
- Secondary: white fill, `#1C2B5E` border, navy text
- Yellow CTA: `#FFC107` fill, `#1C2B5E` text — used for high-urgency enrollment prompts
- Hover: gradient shifts, slight shadow lift

**Course Cards**
- White bg, `#E2E5EE` border, 16px radius, strong drop shadow
- Top: colorful subject illustration (not photography)
- Content: subject name (600), grade level badge, "lessons" count
- Grade badge: rounded pill, subject-specific color

**Subject Illustrations**
- Flat illustration style — custom per subject (Math, Science, English, etc.)
- Bright saturated colors within each illustration
- Not photography — illustrations feel educational and engaging

**Achievement Badges**
- Circular or shield shapes
- Gold `#FFC107` for top tier, silver for mid, green for completion
- Used in student profiles and post-lesson celebrations

**Video Player**
- Full-width with chapter navigation below
- Progress bar in brand navy
- "Ask a doubt" floating button — `#FFC107` bg, navy icon

**Inputs**
- 1px `#E2E5EE` border, 8px radius, 16px padding
- Focus: 2px `#1C2B5E` border
- OTP input: large single-character boxes for phone verification

## Visual Patterns

- Gradient banners (navy-to-purple) on all major sections and CTAs
- "India's #1 Learning App" social proof headline in hero
- Download app CTA with App Store / Play Store badges prominent
- Star tutor profiles — large headshot, student count, subject
- Parent testimonial quotes with photo, city, child's grade
- Learning outcome stats: "42M+ students", "1,700+ cities"
- Grade selector tabs (Class 1–12, JEE, NEET, etc.) on homepage
- Colorful flat-style subject icons in consistent style

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 150ms | Button hover, focus |
| Duration base | 300ms | Card hover, dropdown, modal |
| Duration slow | 500ms | Page transitions, hero load |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | All transitions |

Confetti/celebration animation on lesson completion. Smooth gradient shift on CTA button hover. Entrance animations for stats (count-up) in hero section. Card hover lifts with shadow and slight scale (1.02).
