# Shopify Design Language

## Aesthetic
Merchant-first, calm, actionable. Light interface built for hours of daily use — nothing should tire the eyes. Green brand (Shopify green) on white. Polaris Design System. Every element communicates trust and clarity. No visual noise.

## Color Usage
- **Page bg**: `#FFFFFF`
- **Secondary bg**: `#F1F1F1`
- **Surface**: `#FAFAFA`
- **Selected/active**: `#EBF9F5` (tinted green)
- **Text primary**: `#202223`
- **Text secondary**: `#6D7175`
- **Text disabled**: `#8C9196`
- **Border default**: `#C9CCCF`
- **Border subdued**: `#E4E5E7`
- **Brand**: `#008060` (Shopify green)
- **Interactive**: `#0070F0` (blue — links, focus)
- **Success**: `#008060`, bg `#AEE9D1`
- **Warning**: `#B98900`, bg `#FFEA8A`
- **Critical**: `#D72C0D`, bg `#FED3D1`
- **Info**: `#0070F0`, bg `#D5E8FF`

## Typography
- Font: **Inter** (fallback: SF Pro, Segoe UI)
- Admin UI body: 14px, weight 400, line-height 1.5
- Page titles: 20px, weight 600
- Section headings: 16px, weight 600
- Labels: 14px, weight 500
- Captions: 12px, `#6D7175`
- Mono: SFMono-Regular, Consolas

## Spacing
4px base. Admin uses 16–20px page padding. Cards: 20px internal padding. Table rows: 12px vertical. Form field gaps: 16px.

## Layout
- **Admin shell**: left nav (240px) + main content
- Nav bg: white with `border-right: 1px solid #E4E5E7`
- Content: max 1000px centered with `padding: 0 20px`
- **Page header**: title + breadcrumb + action buttons (top right)

## Components

### Navigation (admin left)
- Logo: 56px height top
- Nav items: 36px height, 8px 12px padding, `border-radius: 8px`
- Hover: `#F1F1F1`; Active: `#EBF9F5` bg, `#008060` text
- Section headers: 12px, `#6D7175`, uppercase
- Badge counts: `#D72C0D` red dot or number badge

### Cards (Polaris)
- `border: 1px solid #E4E5E7`, `border-radius: 8px`, bg `#FFFFFF`
- Shadow: `0 0 0 1px rgba(63,63,68,0.05), 0 1px 3px 0 rgba(63,63,68,0.15)`
- Section header inside card: `border-bottom: 1px solid #E4E5E7`, 12px 20px padding
- Content: 20px padding

### Buttons
- Primary: `#008060` bg, white text, `border-radius: 8px`
- Default: white bg, `#C9CCCF` border, `#202223` text
- Destructive: `#D72C0D` bg
- Height: 36px, font: 14px weight 500
- Disabled: `#F1F1F1` bg, `#8C9196` text

### Data tables
- Header: 14px weight 600, `#6D7175`, `#F6F6F7` bg
- Row: 48px height, `border-bottom: 1px solid #E4E5E7`
- Hover row: `#F6F6F7` bg
- Checkbox: left of row, shows on hover
- Sortable columns: up/down arrow on hover

### Form fields
- Label: 14px weight 500, `#202223`
- Input: `border: 1px solid #C9CCCF`, `border-radius: 4px`, 36px height
- Focus: `border-color: #458FFF`, `box-shadow: 0 0 0 3px #458FFF33`
- Error: `border-color: #D72C0D`, error message below in red
- Help text: 13px `#6D7175` below field

### Status badges
- Pill shape `border-radius: 20px`, 12px 8px padding
- Success: `#AEE9D1` bg, `#004F43` text
- Warning: `#FFEA8A` bg, `#4C3200` text  
- Critical: `#FED3D1` bg, `#7B1F12` text
- Info: `#D5E8FF` bg, `#0A2E68` text

### Banners
- Full-width inside page content, `border-radius: 8px`
- Left border 4px colored by type
- Icon left, content right, dismiss X far right

## Visual Patterns
- **Product images**: square aspect ratio, checkerboard bg for transparent
- **Analytics charts**: line/bar in Shopify green, clean axes
- **Order timeline**: vertical left line + event dots
- **Bulk actions**: toolbar appears when rows selected, slides in from bottom
- **Empty states**: centered illustration (abstract shapes) + heading + CTA

## Motion
- Duration: 200ms default
- Easing: ease-in-out
- Page transitions: fade content
- Toast: slide up from bottom-center, auto-dismisses 3s
