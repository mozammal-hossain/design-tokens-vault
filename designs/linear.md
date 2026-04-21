# Linear Design Language

## Aesthetic
Dark, dense, fast. Feels like a tool built for power users. Near-black backgrounds, subtle purple brand, crisp Inter typography. No unnecessary decoration. Every pixel earns its place. Speed is the brand.

## Color Usage
- **Page bg**: `#0F0F11` (near black, not pure black)
- **Secondary bg**: `#18181B`
- **Surfaces**: `#1E1E22` cards, `#26262B` on hover
- **Text**: `#F4F4F5` primary, `#A1A1AA` secondary, `#71717A` tertiary
- **Brand**: `#5E6AD2` (muted purple-indigo) — used sparingly for links, focus, active states
- **Borders**: `#27272A` (1px, barely visible)
- **Status labels**: full color palette — purple, blue, green, yellow, red, orange

## Typography
- Font: **Inter**, system-ui fallback
- UI text: 13–14px base, tight and dense
- Headlines: 22–28px, weight 600, letter-spacing `-0.01em`
- Mono (code/IDs): IBM Plex Mono or Fira Code, 12–13px
- All text anti-aliased with high contrast against dark surfaces

## Spacing
4px base unit. Dense compact UI — 8–12px padding inside components. Sidebar items: 6px 8px. List rows: 8px vertical padding. Section gaps: 24–32px.

## Layout
- 3-column app shell: narrow sidebar (240px) + content list (340px) + detail panel (flex)
- Sidebar: `#18181B`, collapsible
- Content area scrolls independently
- No external marketing-style padding — content fills space

## Components

### Sidebar
- `#18181B` bg, 240px wide
- Items: 28px height, 8px 12px padding, `border-radius: 6px`
- Active item: `#26262B` bg with `#5E6AD2` left indicator
- Section headers: 11px, weight 600, `#71717A`, uppercase

### Issue/Item Rows
- Full-width, 40px height, 1px bottom border `#27272A`
- Status dot (colored circle, 8px) + title + metadata right-aligned
- Hover: `#26262B` bg, smooth 80ms
- Checkbox appears on hover

### Buttons
- Primary: `#5E6AD2` bg, white text, `border-radius: 6px`, 8px 16px
- Secondary: `#26262B` bg, `#B3B3B3` text, 1px border `#3F3F46`
- Ghost: transparent, text only, hover shows bg
- Height: 32px (compact), 36px (default)

### Inputs / Command palette
- Command palette: `#1E1E22` bg, `border: 1px solid #27272A`, shadow `0 16px 70px rgba(0,0,0,0.6)`
- Search input: `border-radius: 8px`, 16px padding, 40px height
- Results: 36px rows, keyboard-navigable highlight `#26262B`

### Labels / Badges
- Small pills: `border-radius: 4px`, 4px 8px padding, 11px text
- Each status color has bg (10% opacity) + text (full color)

### Priority indicators
- Urgent: red dot; High: orange; Medium: yellow; Low: gray
- Consistent 8px circles, placed before title

## Visual Patterns
- **Keyboard-first**: visible keyboard shortcuts on hover throughout
- **Empty states**: minimal — single icon + short text, no illustrations
- **Loading states**: skeleton screens with `#26262B` shimmer
- **Modals**: centered, dark bg, subtle border, strong backdrop blur
- **Avatars**: small (20px), circular, grayscale by default
- **Icons**: 16px, thin stroke, Lucide or similar

## Motion
- Duration: 80ms fast, 150ms default — extremely snappy
- Spring easing on dialogs: `cubic-bezier(0.34, 1.56, 0.64, 1)`
- List items: stagger fade-in on page load (30ms between items)
- No decorative animations — only functional transitions
