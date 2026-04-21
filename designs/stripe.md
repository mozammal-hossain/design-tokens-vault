# Stripe Design Language

## Aesthetic
Clean, trustworthy, premium fintech. Heavy use of white space. Subtle gradients and depth. Feels engineered and precise. Dark navy text on white — never harsh black. Purple-indigo brand anchors calls to action.

## Color Usage
- **Page bg**: `#FFFFFF` with `#F6F9FC` offset sections
- **Body text**: `#0A2540` (dark navy, not black)
- **Secondary text**: `#425466`
- **Brand CTA**: `#635BFF` buttons, links, highlights
- **Borders**: `#E6EBF1` (very subtle)
- **Status colors**: muted, accessible — green `#09825D`, red `#C0392B`

## Typography
- Font: **Sohne** (fallback: Helvetica Neue, Arial)
- Headlines: large, tight letter-spacing (`-0.02em`), weight 600–700
- Body: 16px, weight 400, line-height 1.5
- Labels/captions: 12–14px, weight 500, slightly tracked
- Code: Sohne Mono

## Spacing
4px base unit. Sections breathe — 80–96px vertical padding. Cards use 24–32px internal padding. Tight grids (12–16px gaps).

## Layout
- Max content width: 1080px, centered
- Hero: full-width, 2-col (text left, illustration/demo right)
- Feature sections alternate side-by-side and centered
- Dashboard previews float with layered card shadows

## Components

### Buttons
- Primary: `#635BFF` bg, white text, `border-radius: 6px`, 12px 20px padding
- Secondary: white bg, `#0A2540` border, same radius
- Hover: darken brand `→ #4F46E5`, smooth 200ms transition
- Focus ring: `0 0 0 3px rgba(99,91,255,0.25)`

### Cards
- White bg, `border: 1px solid #E6EBF1`, `border-radius: 8px`
- Shadow: `0 4px 16px rgba(0,0,0,0.08)`
- Hover: lift shadow to `0 8px 32px rgba(0,0,0,0.12)`

### Inputs
- Height: 40px, `border: 1px solid #E6EBF1`, radius 6px
- Focus: border `#635BFF`, shadow `0 0 0 3px rgba(99,91,255,0.25)`
- Placeholder: `#9BAFC2`

### Navigation
- Sticky, white bg on scroll with shadow `0 1px 0 #E6EBF1`
- Links: `#425466`, hover `#0A2540`
- CTA button in nav: solid brand purple

### Code blocks
- `#0A2540` bg, Sohne Mono 13px, syntax highlighting with brand purples

## Visual Patterns
- **Gradient mesh backgrounds** in hero sections — subtle purple/blue/teal blends
- **Floating UI mockups** with drop shadows showing product dashboards
- **Animated gradients** on hero text
- **Icon style**: thin stroke, 1.5px, rounded caps
- **Section dividers**: background color shift, no hard lines
- **Illustrations**: isometric product UI screenshots, not custom art

## Motion
- Duration: 200ms default, 100ms micro-interactions
- Easing: `cubic-bezier(0.25, 0.46, 0.45, 0.94)`
- Hover transitions on all interactive elements
- Page sections: fade-in + slide-up on scroll (subtle, 20px travel)
