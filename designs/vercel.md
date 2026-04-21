# Vercel Design Language

## Aesthetic
Dark, minimal, developer-focused. Pure black and white with rare color accents. Feels like a terminal elevated into a product. Geist typeface (Vercel's own). Precision over decoration. High contrast, no noise.

## Color Usage
- **Page bg**: `#000000` (true black)
- **Secondary bg**: `#0A0A0A`
- **Surface**: `#111111` cards/panels
- **Hover**: `#1A1A1A`
- **Text**: `#FFFFFF` primary, `#888888` secondary, `#666666` tertiary
- **Borders**: `#333333` default, `#222222` subtle
- **Accent blue**: `#0070F3` — primary interactive color, links, focus
- **Accent violet**: `#7928CA` — gradient pair with blue
- **Status green**: `#0EB360`, red: `#FF4444`, yellow: `#F5A623`

## Typography
- Font: **Geist** (Vercel's typeface, fallback to system-ui)
- Mono: **Geist Mono** for all code
- Hero headlines: 48–64px, weight 700, letter-spacing `-0.02em`
- Section headings: 28–36px, weight 600
- Body: 14–16px, weight 400, line-height 1.5
- Labels: 12–13px, weight 500

## Spacing
4px base. Compact dense UI in dashboard. Marketing pages: 80px section padding. Cards: 16–24px internal padding. Grid gaps: 16px.

## Layout
- **Dashboard**: left sidebar (232px, `#000`) + content area (flex)
- **Marketing pages**: centered, max 1200px
- **Hero**: centered text, no image — relies on typography weight alone
- **Feature grid**: 2–3 column cards

## Components

### Buttons
- Primary: white bg, black text, `border-radius: 6px`, `border: 1px solid #333`
- CTA: `#0070F3` bg, white text
- Ghost: transparent, white text, `border: 1px solid #333`
- Height: 32px (small), 40px (default)
- Hover: bg lightens slightly, border brightens

### Cards
- `#111111` bg, `border: 1px solid #333`, `border-radius: 8px`
- Hover: border `#555`
- Shadow: `0 4px 16px rgba(0,0,0,0.6)`
- Inner content padding: 20–24px

### Inputs
- `#000` bg, `border: 1px solid #333`, `border-radius: 6px`
- Text: `#EAEAEA`, placeholder `#444`
- Focus: border `#0070F3`, shadow `0 0 0 2px rgba(0,112,243,0.4)`
- Height: 36px

### Navigation (Dashboard)
- Left sidebar: `#000` bg, 232px
- Nav items: 36px height, 8px 12px padding, `border-radius: 6px`
- Active: `#111` bg, white text
- Hover: `#0A0A0A`
- Section labels: 11px, `#666`, uppercase, tracking wide

### Deployment status badges
- Success: `#0EB360` dot + text
- Building: `#F5A623` animated pulse dot
- Error: `#FF4444` dot
- Always monospace for hashes and timestamps

### Code blocks / Terminal
- `#0A0A0A` bg or true `#000`
- Geist Mono 13px
- Syntax: blue for keywords, green for strings, orange for values
- Window chrome: three dots + filename tab

### Tables
- `#111` rows, `border-bottom: 1px solid #222`
- Header: 11px uppercase, `#666`, weight 600
- Hover row: `#1A1A1A`

## Visual Patterns
- **Gradient text** on hero: `#0070F3 → #7928CA` (blue to violet)
- **Glow effects**: `box-shadow: 0 0 20px rgba(0,112,243,0.3)` on accent elements
- **Edge/serverless indicators**: small colored dots in deployment tables
- **CLI snippets**: dark terminal blocks with colored output lines
- **Monospace timestamps** everywhere — dates shown as relative + absolute on hover
- **Animated deploy progress**: step-by-step with connecting lines

## Motion
- Duration: 100ms fast, 200ms default
- Spring bounce: `cubic-bezier(0.34, 1.56, 0.64, 1)` on modals/dropdowns
- Skeleton loading: dark shimmer `#111 → #1A1A1A`
- Page transitions: instant (Next.js client navigation)
