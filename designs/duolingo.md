# Duolingo — Design Language

## Aesthetic

Playful, gamified, and habit-forming. Duolingo is the most distinctly branded edtech product — its design is closer to a mobile game than a learning platform. The owl mascot (Duo), electric green brand color, chunky rounded buttons with hard drop shadows, and bright accent colors create an instantly recognizable system. The design rewards consistency with streaks, XP, and leagues. Everything is designed to feel like a game that happens to teach you a language.

## Color Usage

| Role | Hex | Usage |
|------|-----|-------|
| Brand Green | `#58CC02` | Primary buttons, correct answer, progress, brand elements |
| Brand Dark | `#46A302` | Button shadow/border (the "3D" press effect base) |
| Brand Light | `#D7F5B1` | Correct answer bg, success states |
| Brand Push | `#89E219` | Hover state of brand buttons |
| Accent Blue | `#1CB0F6` | Secondary actions, info, "Super" subscription |
| Accent Red | `#FF4B4B` | Incorrect answers, heart/lives lost, error states |
| Accent Orange | `#FF9600` | Streaks, fire icon, urgency |
| Accent Purple | `#CE82FF` | Legendary league, premium features |
| Accent Yellow | `#FFC800` | XP badges, crowns, achievements |
| Background | `#FFFFFF` | Primary light mode page background |
| Background Secondary | `#F7F7F7` | Section fills, sidebar |
| Background Dark | `#131F24` | Dark mode primary background |
| Text Primary | `#3C3C3C` | All body text and headings |
| Text Secondary | `#777777` | Meta, captions, secondary info |
| Text on Dark | `#FFFFFF` | Text on dark backgrounds |
| Border | `#E5E5E5` | Card borders, dividers |
| Border Strong | `#AFAFAF` | Buttons border (unfocused), input borders |
| Success | `#58CC02` | Correct answer indicator |
| Error | `#FF4B4B` | Wrong answer indicator |
| Warning | `#FF9600` | Streak warning, lives low |
| Streak | `#FF9600` | Streak count and flame |
| XP Gold | `#FFC800` | XP amount displays, crown icons |

## Typography

**Font:** Nunito — rounded, friendly, and bold-capable. The rounded terminals reinforce the playful character. Heavy weights (800) used in headings.

| Role | Size | Weight | Line Height |
|------|------|--------|-------------|
| Display / hero | 40px | 800 | 1.2 |
| Section heading | 32px | 800 | 1.2 |
| Card heading | 24px | 700 | 1.3 |
| Body | 17px | 400 | 1.5 |
| Small body | 15px | 400 | 1.5 |
| Label / badge | 13px | 700 | 1.2 |

## Spacing

Base unit: 4px.

| Token | Value | Usage |
|-------|-------|-------|
| 2xs | 4px | Icon gaps, micro-spacing |
| xs | 8px | Badge padding, tag gaps |
| sm | 12px | List item padding, chip padding |
| md | 16px | Card padding, input spacing |
| lg | 24px | Component spacing |
| xl | 32px | Section spacing |
| 2xl | 48px | Section padding |
| 3xl | 64px | Major section separators |

## Layout

- Mobile-first: primary experience is the iOS/Android app
- Web app: max 700px content column, centered, generous side margins
- Lesson view: single question centered, progress bar top, answer options below
- Home: left sidebar (navigation), center (lesson tree), right (streak/league sidebar)
- Lesson tree: vertical branching path with unit nodes

## Components

**Buttons (the signature Duolingo button)**
- Primary: `#58CC02` fill, white text, pill/20px radius, 800 weight
- Hard drop shadow at bottom: `0 4px 0 #46A302` — creates a "3D press" illusion
- On press: shadow removed, button shifts 4px down — tactile response
- Hover: `#89E219` bg
- Secondary: white fill, `#AFAFAF` border (2px), `#3C3C3C` text, same shadow style
- Disabled: `#E5E5E5` fill, `#AFAFAF` text, no shadow

**Answer Option Buttons**
- Same pill style as secondary button
- Correct: `#D7F5B1` bg, `#58CC02` border (3px), green checkmark
- Incorrect: `#FFE8E8` bg, `#FF4B4B` border (3px), red X mark
- Selected: `#DDF4FF` bg, `#1CB0F6` border (3px)

**Progress Bar (XP / Lesson)**
- `#58CC02` fill on `#E5E5E5` track
- 16px height (prominent), 8px radius
- Animated fill with easing on progress

**Streak Display**
- Orange flame icon (`#FF9600`) + bold number count
- Streak freeze: ice/blue variant
- Displayed in: header, profile, daily goal section

**XP / Achievement Badge**
- Gold circle `#FFC800`, bold number or icon inside
- "League" badges: Bronze, Silver, Gold, Sapphire, Ruby, Emerald, Amethyst, Pearl, Obsidian, Diamond — each with custom colors

**Heart / Lives Display**
- Red heart icons (`#FF4B4B`), filled = remaining lives
- Lost: gray outline heart
- 5 lives max in free tier

**Course Tree Nodes**
- Circular nodes, 64px diameter
- Active: brand green, glow shadow
- Completed: filled with star/crown based on mastery
- Locked: `#E5E5E5` gray fill

**Duo Mascot**
- The green owl character appears throughout — lesson complete, streak reminders, error states
- Mascot has expressive face states: happy, sad, angry, surprised, encouraging

## Visual Patterns

- Gamification layer is inseparable from the learning experience
- Daily goal circle with progress ring (`#58CC02`)
- League leaderboard — top 10 users with XP counts, trophy positions
- "Streak at risk" reminder — orange warning with flame
- "Perfect lesson" celebration: Duo mascot + confetti burst
- Badge collection page — grid of earned achievements
- Lingots/Gems currency display (in-app store)
- Bold, flat illustrations throughout — no photography
- Emoji-style character sets for language exercises
- Challenge complete screen: full-screen celebration with Duo dancing

## Motion

| Property | Value | Usage |
|----------|-------|-------|
| Duration fast | 100ms | Button press (shadow removal = instant tactile feel) |
| Duration base | 200ms | Correct/incorrect reveal, progress bar |
| Duration slow | 400ms | Celebration screens, mascot entry |
| Easing standard | `cubic-bezier(0.4, 0, 0.2, 1)` | Standard transitions |
| Easing bounce | `cubic-bezier(0.34, 1.56, 0.64, 1)` | Correct answer, achievement earn, badge unlock |

Confetti burst on lesson completion. Duo mascot animates (bounce/wave) on celebrations. XP counter animates upward on earn. Streak flame pulses. Button press is instant (0ms) to maximize tactile feel. Progress bar fills with smooth easing after each correct answer.
