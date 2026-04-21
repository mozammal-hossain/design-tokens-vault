# Notion Design Language

## Aesthetic
Minimal, paper-like, calm. Feels like a blank canvas. Off-white backgrounds, warm dark text (`#37352F` not pure black). Everything is content-first — chrome disappears until needed. Supports both light and full dark mode.

## Color Usage
- **Light bg**: `#FFFFFF`, offset sections `#F7F6F3` (warm off-white)
- **Dark bg**: `#191919`
- **Text (light)**: `#37352F` (warm dark brown-black)
- **Text (dark)**: `rgba(255,255,255,0.81)`
- **Secondary text**: `#787774`
- **Borders**: `#E9E9E7` light, `#424242` dark — very quiet
- **Brand blue**: `#2EAADC` — only for links and selection
- **Text highlight palette**: 10 colors (gray/brown/orange/yellow/green/blue/purple/pink/red) as `#F*` soft backgrounds

## Typography
- Font: system-ui stack (`ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI"`)
- Supports serif and mono as alternative page fonts
- H1: 40px, weight 700, line-height 1.2
- H2: 30px, weight 600
- H3: 24px, weight 600
- Body: 16px, weight 400, line-height 1.75 (generous reading rhythm)
- Caption: 14px, `#787774`

## Spacing
4px base. Page content max-width 708px (default), 900px (wide). Content has 96px horizontal padding on desktop. Block spacing: 2px between same-type blocks, 12px between sections.

## Layout
- **Sidebar**: 240px, `#F7F6F3` bg light / `#2F2F2F` dark, collapsible
- **Content**: centered column, max 708px, full scrolling
- **Top bar**: 45px height, sticky, shows breadcrumb + actions
- **Cover image**: full-width banner, 20% height of viewport

## Components

### Blocks
- All content is blocks — hover reveals drag handle (⋮⋮) on left, action menu (+) far left
- Block padding: 1px 2px
- Inline editing: click anywhere to focus, no input chrome until active
- Selection: `rgba(46,170,220,0.15)` background highlight

### Buttons
- Small, minimal — `border-radius: 3px`, 6px 10px padding, 14px text
- Primary: `#2EAADC` — rare, only major actions
- Secondary: `#F1F1EF` bg, `#37352F` text
- Hover: darken bg by 5%

### Database views (Table/Board/Gallery/Calendar)
- Table: 1px `#E9E9E7` row/column borders, 32px row height
- Board: Kanban columns 260px wide, cards with 8px radius and subtle border
- Gallery: card grid, 16px gap, images fill card top
- Property badges: 6px radius pills, muted background per type

### Sidebar items
- 28px height, `border-radius: 3px`
- Active: `rgba(0,0,0,0.05)` bg
- Nested indent: 12px per level
- Emoji icon (16px) before page title

### Slash menu / Quick menu
- `border-radius: 4px` dropdown, white bg with `rgba(15,15,15,0.1)` shadow
- 36px rows, icon left + label + description right
- Search filters list in real-time

### Highlight colors
- Applied as bg color behind text inline
- 10 named colors, pastel range, readable at all weights

## Visual Patterns
- **Emoji as icons** — pages, databases, workspace sections all use emoji
- **Cover photos** — Unsplash-sourced, gradient, or solid color banners
- **Inline linked pages** — hover preview card with shadow
- **Property types** — each has a distinct icon (calendar, person, select, etc.)
- **Empty state**: big emoji + short italic hint text
- **Templates gallery**: card grid with preview thumbnails

## Motion
- Transitions: 250ms, ease
- Sidebar: slide in/out on toggle
- Block drag: smooth reorder with placeholder
- Page navigation: near-instant (no loading states for local content)
