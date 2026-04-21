# Framer Design Language

## Aesthetic
Design tool meets no-code website builder. Clean black/white with electric blue accent. Dark editor panels. Marketing site is bold and typographic — large Inter headings, minimal imagery, gradient accents. Feels cutting-edge and creative-professional.

## Color Usage
- **Light bg**: `#FFFFFF`
- **Dark bg**: `#111111`
- **Editor panels**: `#1C1C1C`
- **Surface (light)**: `#F5F5F5`
- **Surface (dark)**: `#1C1C1C`
- **Surface hover (light)**: `#EBEBEB`
- **Surface hover (dark)**: `#252525`
- **Text (light)**: `#111111`
- **Text (dark)**: `#FFFFFF`
- **Secondary (light)**: `#666666`
- **Secondary (dark)**: `#999999`
- **Border (light)**: `#E5E5E5`
- **Border (dark)**: `#333333`
- **Brand blue**: `#0055FF`
- **Brand hover**: `#0044CC`
- **Gradient start**: `#0055FF`; end: `#9B51E0`
- **Blue glow**: `rgba(0,85,255,0.2)`
- **Success**: `#00CC66`; error: `#FF3333`
- **Selection**: `#0055FF`

## Typography
- Font: **Inter** (UI), **Framer Sans** for display (when available)
- Marketing H1: 48–72px, weight 700, letter-spacing `-0.02em`, line-height 1.1
- Section H2: 28–40px, weight 600
- Body: 16px, weight 400, line-height 1.5
- Editor UI: 12–14px, Inter
- Captions: 13px, `#666666`
- Code: 13px mono

## Spacing
4px base. Marketing sections: 80–120px vertical padding. Editor: 8px panel padding. Component gaps: 16px. Max content: 1100px.

## Layout
- **Editor**: toolbar top (40px) + canvas center + left panel (260px, layers) + right panel (260px, properties)
- **Marketing**: full-width sections, centered text, no rigid grid
- **Templates gallery**: responsive card grid

## Components

### Canvas (editor)
- `#F5F5F5` canvas with grid dots option
- Frame borders: blue `#0055FF` handles on selection
- Element handles: white squares at corners/edges, 6px
- Distance labels: appear between elements on hover (blue dimension lines)
- Breakpoint switcher: desktop/tablet/mobile icons in toolbar

### Property panel (right)
- Dark `#1C1C1C` bg
- Section headers: 11px uppercase `#666666`
- Inputs: 28px height, `#2A2A2A` bg, 12px font
- Color swatch: 16px square, `border-radius: 3px`
- All values editable inline

### Layers panel (left)
- Dark `#1C1C1C` bg
- Page name at top, layer tree below
- 24px row height
- Frame: blue icon; component: purple; text: T; image: landscape icon
- Indent per level: 12px
- Hover: `#252525`; selected: `rgba(0,85,255,0.2)`

### Marketing buttons
- Primary: `#0055FF` bg, white, `border-radius: 9999px`, `px-6 py-3`
- Secondary: white bg, `#111` border, same radius
- CTA large: 52px height, 18px font, weight 700
- Hover: blue darkens, slight scale 1.01

### Cards (templates/sites)
- `border-radius: 12px`
- Image fills card, no bg
- Hover: scale 1.02, border `1px solid #E5E5E5`
- Below: title 16px 600 + category tag

### Glow effects
- Blue glow on hero elements: `box-shadow: 0 0 40px rgba(0,85,255,0.2), 0 0 80px rgba(0,85,255,0.1)`
- Applied to hero product screenshots or CTAs

### Code component editor
- Dark code block, syntax highlighted
- `#1C1C1C` bg, `border-radius: 8px`
- Framer-specific: JSX with motion imports highlighted

### Component store
- Search + filter sidebar
- Cards: preview image + name + author + price
- Featured: hero banner with gradient

## Visual Patterns
- **Gradient text**: headings use `background-clip: text` with `#0055FF → #9B51E0`
- **Site preview cards**: mini browser mockup with live interaction
- **AI features**: sparkle icon, gradient treatment
- **Motion principles**: easing curve visualizer in properties
- **Scroll interactions**: timeline-based with scrub preview
- **Smart components**: variant swapping with visual diff

## Motion
- Editor interactions: instant
- Marketing reveals: fade + translateY(20px), 400ms ease-out on scroll
- Blue glow pulse: `@keyframes pulse 2s infinite` on hero accents
- Card hover: 150ms scale ease-out
- Spring: `cubic-bezier(0.34, 1.56, 0.64, 1)` on modals + panels
