# Uber Design Language

## Aesthetic
Bold, black-and-white, functional. Uber Move typeface is the brand. Maximum contrast — pure black on white, pure white on black. Very little color noise; green for positive/driver, red for negative/cancel. Feels like a utility built for speed and clarity.

## Color Usage
- **Light bg**: `#FFFFFF`
- **Dark bg**: `#000000`
- **Secondary bg (light)**: `#F6F6F6`
- **Secondary bg (dark)**: `#1A1A1A`
- **Surface (light)**: `#EEEEEE`
- **Surface (dark)**: `#262626`
- **Text (light)**: `#000000`
- **Text (dark)**: `#EEEEEE`
- **Secondary text (light)**: `#545454`
- **Secondary text (dark)**: `#ABABAB`
- **Disabled**: `#B2B2B2`
- **Accent green**: `#06C167` (driver/positive states)
- **Negative**: `#E11900`
- **Warning**: `#FFC043`
- **Promo**: `#9747FF`
- **Border (light)**: `#E2E2E2`

## Typography
- Font: **Uber Move** (fallback: system-ui)
- Mono: **Uber Move Mono** for fare amounts, ETAs
- App headings: 24–32px, weight 700, letter-spacing `-0.01em`
- Button labels: 16px, weight 700
- Body: 16px, weight 400
- Captions/metadata: 12–14px, `#545454`
- Fare display: 32–40px, weight 700, Uber Move

## Spacing
4px base. Map takes 50–60% of app viewport. Bottom sheet: 24px padding. Card padding: 16px. Button height: 52px (large touch targets for in-car use).

## Layout
- **App (mobile)**: map fills top 60%, bottom sheet slides up with options
- **Driver app**: similar but inverted importance
- **Web**: standard 1200px max, centered, minimal nav
- **Bottom sheet states**: collapsed (just search bar) → peek (options) → full (fare breakdown)

## Components

### Map view
- Full-bleed map (Mapbox/Google)
- Uber-branded custom map style: desaturated streets, bold road labels
- Pickup pin: black circle with white outline
- Dropoff pin: solid black square
- Driver icon: car top-down view
- Surge zone overlay: orange heat tint

### Search / Destination input
- Pill input: `border-radius: 9999px`, 56px height, white bg, shadow
- Origin dot (gray) + destination dot (black) with vertical connector line
- Recent locations below with clock icon

### Vehicle options (ride selection)
- Horizontal scroll row OR vertical list
- Each option: car icon + name + capacity + ETA + price
- Active: bold black border `2px solid #000`
- Card: `border-radius: 8px`, 64px height

### Buttons
- Primary: `#000000` bg, `#FFFFFF` text, `border-radius: 8px`
- Secondary: `#FFFFFF` bg, `#000000` border + text
- Danger: `#E11900` bg, white text
- Height: 52px (app), 44px (web)
- Font: 16px, weight 700

### Driver card (active ride)
- `border-radius: 16px`, white bg, shadow
- Driver photo (48px circle) + name + rating + vehicle
- Call / Message icons right
- Car plate: monospaced
- Green progress track showing driver approach

### Fare breakdown
- Clean list: items left, prices right
- Total: bold, larger, with separator line above
- Currency: Uber Move Mono

### Rating flow
- 5 stars: `#000000` filled stars
- Default: `#E2E2E2` outline
- Taps select left-to-right

### Status pills
- Arriving: `#000000` bg, white text
- `border-radius: 9999px`, 12px 16px padding, 14px weight 700

## Visual Patterns
- **Surge pricing**: orange badge on vehicle option
- **Scheduled rides**: calendar icon, blue time badge
- **Promotions**: `#9747FF` promo badge, "$X off" pill
- **Safety features**: SOS button, share trip, trusted contacts
- **Driver ETA**: real-time countdown, large and prominent
- **Receipt**: clean list layout, receipt-paper aesthetic

## Motion
- Map: smooth camera fly to location on selection
- Bottom sheet: spring physics slide up
- Car icon: smooth GPS-tracked movement
- Fare estimate: number count-up animation
- Arrival: pulsing ring around driver pin
