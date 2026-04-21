# Khan Academy — Design Language

## Aesthetic

Friendly, open, and empowering. Khan Academy's design is warm and approachable without being childish — it must serve learners from age 6 to adult. The green brand color signals growth and positive reinforcement. White space is generous. The overall feel is welcoming and trustworthy, with subtle gamification elements (points, streaks, badges) that motivate without overwhelming.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand Green | `#14BF96` | Primary buttons, progress, success states, mastery fills |
| Brand Dark | `#0D8A6A` | Button hover, active nav |
| Brand Light | `#E7F8F4` | Backgrounds for success states, selected items |
| Accent Blue | `#1865F2` | Links, secondary CTAs, info states |
| Accent Gold | `#FFB100` | Streaks, energy points, achievement badges |
| Background | `#FFFFFF` | Page and card backgrounds |
| Background Secondary | `#F7F8FA` | Section fills, sidebar, content panels |
| Background Dark | `#21242C` | Footer, dark sections |
| Text Primary | `#21242C` | All headings and body copy |
| Text Secondary | `#626975` | Meta text, captions, hints |
| Text Link | `#1865F2` | Inline links, interactive labels |
| Text on Dark | `#FFFFFF` | Text over dark backgrounds |
| Border | `#DBDCDD` | Cards, inputs, dividers |
| Success | `#14BF96` | Mastery, correct answers |
| Warning | `#FFB100` | Near-deadline, review needed |
| Error | `#D92916` | Incorrect answers, validation errors |

## Typography

**Font:** Lato — humanist sans-serif with warmth. Bold weights used heavily in headings. Black (900) weight for display text.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Display / hero | 48px | 900 | 1.25 |
| Section heading | 36px | 700 | 1.25 |
| Card heading | 22px | 700 | 1.3 |
| Body | 16px | 400 | 1.6 |
| Small body | 14px | 400 | 1.6 |
| Caption / hint | 13px | 400 | 1.6 |
| Badge / label | 12px | 700 | 1.25 |

## Spacing

Base unit: 4px. Follows an 8px grid for components, 4px for micro-spacing.

| Token | Value | Usage |
|-------|-------|-------|
| 2xs | 4px | Icon-text gap, inline spacing |
| xs | 8px | Badge padding, list item gaps |
| sm | 12px | Input padding |
| md | 16px | Card inner padding |
| lg | 24px | Component spacing |
| xl | 32px | Section spacing |
| 2xl | 48px | Section padding |
| 3xl | 64px | Major section separators |
| 4xl | 96px | Hero section top/bottom |

## Layout

- Max content width: 1200px, centered
- Left sidebar navigation (260px) for subject browsing
- Main content area fluid with max 720px for readable text
- Mastery grid: skill items in responsive wrapping grid
- Progress dashboard: card layout with mastery percentages

## Components

**Buttons**
- Primary: `#14BF96` fill, white text, 6px radius, 700 weight, 40px height
- Secondary: white fill, `#DBDCDD` border, `#21242C` text
- CTA size: 48px height, 16px 24px padding
- Hover: brand-dark `#0D8A6A`, slight shadow lift

**Exercise Cards**
- White bg, `#DBDCDD` border, 6px radius
- Top: subject icon (colored by domain)
- Title, progress bar (mastery %), "# skills" count
- Mastery states: Not started (gray) → Practiced (light green) → Familiar → Proficient → Mastered (full brand green)

**Mastery Bar**
- Segmented bar with 4 states colored from `#E7F8F4` to `#14BF96`
- Width 100%, height 8px, pill radius

**Energy Points Badge**
- Gold `#FFB100` circular badge
- Point count in bold, +N animations on earn
- Position: top-right of user avatar

**Exercise Interface**
- Large centered question text (22px, 700)
- Multiple choice: white pill buttons with `#DBDCDD` border
- Correct: `#E7F8F4` bg, `#14BF96` border, checkmark
- Incorrect: `#FFF0EE` bg, `#D92916` border, X mark
- Hints panel: `#F7F8FA` bg, expandable

**Inputs**
- 1px `#DBDCDD` border, 6px radius, 12px 16px padding
- Focus: 2px `#1865F2` border
- Error: `#D92916` border

## Visual Patterns

- Mascot illustrations (Sal the owl concept) used in empty states and onboarding
- Domain colors: Math (blue), Science (green), Humanities (purple), Computing (teal)
- Achievement badges with illustrated icons, gold/silver/green tiers
- Streak flame icon in `#FFB100` with count
- Video lessons: thumbnail with play button, duration badge
- "Mastered" checkmark animation on completing a skill
- Colorful subject icons — flat style, consistent stroke weight

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 150ms | Button press, focus rings |
| Duration base | 250ms | Card hover, accordion |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | Standard transitions |
| Easing bounce | `cubic-bezier(0.34, 1.56, 0.64, 1)` | Badge earn, mastery celebration |

Celebratory confetti burst on mastery achievement. Point earn counter animates upward. Progress bar fills smoothly with easing. Correct answer check animates in with a small bounce.
