# Apple Design Language

## Aesthetic
Premium, precise, understated. White space as a design element. SF Pro typography carries the whole visual weight. Photography and product renders are the hero. Zero decoration that doesn't serve function. Feels aspirational and quiet simultaneously.

## Color Usage
- **Light bg**: `#FFFFFF`
- **Section alt**: `#F5F5F7` (cool light gray — Apple's off-white)
- **Dark bg**: `#000000`
- **Dark section**: `#1D1D1F`
- **Surface dark**: `#2D2D2F`
- **Text (light)**: `#1D1D1F`
- **Text (dark)**: `#F5F5F7`
- **Secondary (light)**: `#6E6E73`
- **Secondary (dark)**: `#86868B`
- **Links**: `#0066CC` (light), `#2997FF` (dark)
- **Brand blue**: `#0071E3`
- **System red**: `#FF3B30`; green: `#34C759`; orange: `#FF9500`; yellow: `#FFCC00`; purple: `#AF52DE`
- **Borders**: `#D2D2D7` light, `#424245` dark — barely visible

## Typography
- Font: **SF Pro Display** (headings), **SF Pro Text** (body), **SF Mono** (code)
- Fallback: -apple-system, BlinkMacSystemFont
- Hero headline: 56–80px, weight 700, letter-spacing `-0.022em`, line-height 1.07
- Section H2: 40–56px, weight 700, tight spacing
- Section H3: 28–32px, weight 600
- Body: 17px (SF Pro Text spec), weight 400, line-height 1.47
- Captions: 12–14px, `#6E6E73`
- All text rendered with `font-smoothing: antialiased`

## Spacing
4px base. Sections: 100–120px vertical padding. Content max-width: 980px. Products get 28–36px breathing room between content and edges. Typography-heavy sections: 80px top/bottom.

## Layout
- **Marketing pages**: full-width sections, alternating bg colors
- **Hero**: centered or left-aligned text, 100vh with product render
- **Product pages**: single long-scroll narrative
- Nav: translucent blur `backdrop-filter: blur(20px)`, 44px height
- Content columns: rarely more than 2-up on desktop

## Components

### Navigation
- 44px height, `background: rgba(255,255,255,0.85)`, `backdrop-filter: saturate(180%) blur(20px)`
- Black logo left, nav links centered, CTA/cart right
- Links: 12px, `#1D1D1F`, letter-spacing 0
- Mobile: hamburger → full-screen overlay
- Sticky, subtle border-bottom on scroll

### Hero sections
- Full viewport height
- Text: centered or left-bottom
- Product image: absolute or 2-col
- CTA: two links — "Learn more" (blue text link) + "Buy" (blue text link)
- Color chip row on product pages: small circles showing available colors

### Product cards
- Minimal: image top, title + price below
- `border-radius: 18px` card bg (subtle, same as section)
- No explicit border
- Hover: slight scale `1.02`
- Price: 17px, secondary color

### Buttons
- Primary: `#0071E3` bg, white text, `border-radius: 980px` (pill)
- Ghost: transparent, `#0071E3` text, underline hover
- Height: 44px (touch target), padding: 12px 24px
- No border on primary

### Compare table
- Full-width, alternating row colors
- Column headers: product name + price
- Row headers left: feature name
- Checkmarks: `#34C759` filled circle; X: empty
- Highlight column: subtle blue tint

### Footnotes
- Very small (12px), `#6E6E73`
- Asterisk references to legal/disclosure text
- Separated from main content by subtle rule

### Store product page
- Image carousel: full-width, swipe
- Color picker: small circles, active has ring
- Storage/config: horizontal pill buttons
- Add to bag: large full-width `#0071E3` pill button
- Trade-in and monthly installment below

## Visual Patterns
- **Photography scale**: product renders fill most of viewport, extremely high quality
- **Gradient backgrounds**: deep space imagery for Mac/iPhone launch pages
- **Sticky features**: content scrolls while product image stays (parallax)
- **Comparison sliders**: before/after for display/camera improvements
- **Spec callouts**: data labels pointing to product image
- **Video loops**: product reveal animations autoplay muted

## Motion
- Duration: 300–500ms
- Spring: `cubic-bezier(0.34, 1.56, 0.64, 1)` on product pop-ins
- Parallax: product moves slower than text on scroll
- Reveal: fade + slight translateY on section enter
- No aggressive animations — subtle, dignified
