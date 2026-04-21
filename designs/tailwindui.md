# Tailwind UI Design Language

## Aesthetic
Clean, modern, component-showcase. Neutral slate palette with indigo accent. Inter font throughout. Feels like a well-crafted design system reference — the design IS the product. Light and dark mode tokens are first-class. Precision spacing using Tailwind's 4px scale.

## Color Usage
- **Light bg**: `#FFFFFF`, section alt `#F9FAFB` (gray-50)
- **Dark bg**: `#111827` (gray-900)
- **Surface light**: `#F9FAFB` (gray-50)
- **Surface dark**: `#1F2937` (gray-800)
- **Text (light)**: `#111827` (gray-900)
- **Text (dark)**: `#F9FAFB` (gray-50)
- **Secondary text (light)**: `#6B7280` (gray-500)
- **Secondary text (dark)**: `#9CA3AF` (gray-400)
- **Border (light)**: `#E5E7EB` (gray-200)
- **Border (dark)**: `#374151` (gray-700)
- **Brand**: `#6366F1` (indigo-500)
- **Brand hover**: `#4F46E5` (indigo-600)
- **Success**: `#10B981` (emerald-500)
- **Warning**: `#F59E0B` (amber-500)
- **Error**: `#EF4444` (red-500)

## Typography
- Font: **Inter**, ui-sans-serif fallback
- Marketing H1: 48–60px, weight 700–800, letter-spacing `-0.05em`
- Section H2: 30–36px, weight 700
- Card titles: 18–20px, weight 600
- Body: 16px (1rem), weight 400, line-height 1.625
- Small/captions: 14px (0.875rem)
- Mono: ui-monospace, Cascadia Code, Menlo

## Spacing
Tailwind scale (4px base, 0.5-unit increments). Standard page padding: `px-6 sm:px-8`. Section vertical: `py-24 sm:py-32`. Card padding: `p-6`. Grid gaps: `gap-6` or `gap-8`.

## Layout
- Max width: `max-w-7xl` (1280px) centered with `mx-auto`
- Responsive grid: 1 → 2 → 3 → 4 columns with Tailwind breakpoints
- Sidebar layouts: fixed left sidebar + main scrollable content
- Marketing: alternating full-width sections, centered content column

## Components

### Buttons
- Primary: `bg-indigo-600 text-white hover:bg-indigo-500`, `rounded-md`, `px-3.5 py-2.5 text-sm font-semibold`
- Secondary: `bg-white text-gray-900 ring-1 ring-inset ring-gray-300 hover:bg-gray-50`
- Ghost: `text-indigo-600 hover:text-indigo-500`
- Dark variant: each color shifted by 2 shade steps
- Focus ring: `focus-visible:outline-indigo-600`

### Cards
- `bg-white rounded-xl shadow-sm ring-1 ring-gray-900/5`
- Dark: `bg-gray-800 ring-gray-700/5`
- Padding: `p-6`
- Header image: `rounded-t-xl` edge-to-edge
- Hover: `shadow-md` upgrade

### Navigation
- Top nav: `bg-white border-b border-gray-200` 
- Logo left, links center, CTA right
- Mobile: hamburger → full-screen slide-down
- Active link: `text-indigo-600`

### Form inputs
- `block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600`
- Label: `block text-sm font-medium leading-6 text-gray-900`
- Error state: `ring-red-300 focus:ring-red-500`

### Tables
- `min-w-full divide-y divide-gray-300`
- Header: `bg-gray-50 text-xs font-semibold text-gray-900 uppercase`
- Rows: `divide-y divide-gray-200`, hover `bg-gray-50`
- Actions: right-aligned `text-indigo-600 hover:text-indigo-900`

### Badges
- `inline-flex items-center rounded-full px-2.5 py-0.5 text-xs font-medium`
- Colors: green `bg-green-100 text-green-800`, red, yellow, blue, gray
- Dark variants: `-100 → -900` flipped

### Modals / Dialogs
- Backdrop: `fixed inset-0 bg-gray-500/75`
- Panel: `bg-white rounded-xl shadow-2xl max-w-lg w-full`
- Title: 18px semibold; body: 14px gray-500

### Notifications (toast)
- `max-w-sm w-full bg-white shadow-lg rounded-lg ring-1 ring-black/5`
- Icon left (colored by type) + text + close button
- Position: top-right, stacked

## Visual Patterns
- **Component preview cards**: browser-frame mockup containing component
- **Dark/light toggle**: all components shown in both modes side-by-side
- **Copy button**: appears on code block hover
- **Category nav**: sidebar list of component types
- **Responsive indicators**: shows how component looks at each breakpoint
- **Figma badge**: links to corresponding Figma component

## Motion
- Uses Tailwind `transition` utilities: `transition-colors duration-150 ease-in-out`
- Modals: `transition-opacity duration-300 ease-out`
- Menus: `transition ease-out duration-100` (appear), `ease-in duration-75` (leave)
