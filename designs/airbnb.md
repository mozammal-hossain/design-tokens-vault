# Airbnb Design Language

## Aesthetic
Warm, inviting, human. Prioritizes photography. Coral-red brand with clean white space. Circular font gives a friendly rounded feel. Design feels like a premium travel magazine. Minimal chrome — content and listings dominate.

## Color Usage
- **Page bg**: `#FFFFFF`
- **Secondary bg**: `#F7F7F7`
- **Text primary**: `#222222` (near black)
- **Text secondary**: `#717171`
- **Disabled**: `#B0B0B0`
- **Brand**: `#FF385C` (coral red)
- **Brand dark**: `#E31C5F` (hover/press)
- **Borders**: `#DDDDDD` — clean and light
- **Focus**: `#222222` (inverts to black for accessibility)
- **Success**: `#00A699` (teal)
- **Rating star**: `#FF385C` (brand red stars, not yellow)

## Typography
- Font: **Circular** (fallback: Roboto, Helvetica)
- Hero: 40–64px, weight 700–800, tight line-height 1.2
- Section headings: 24–32px, weight 600
- Listing titles: 16–18px, weight 600
- Body/descriptions: 16px, weight 400, line-height 1.6
- Price: 16px weight 600, per-night rate prominent
- Captions: 14px, `#717171`

## Spacing
4px base. Search bar dominates the header. Content sections: 48px vertical gap. Cards: 12px gap in grid. Internal card padding: none (edge-to-edge image). Below image: 12–16px padding.

## Layout
- **Homepage**: full-width hero with search bar + category pills scroll
- **Search results**: sticky filter bar + 2-col split (map right, listings left)
- **Listing page**: image grid (hero + 4 thumbnails) + 2-col content
- **Content column**: 60% detail, 40% booking card (sticky)
- **Footer**: multi-column links, very minimal

## Components

### Search bar
- Pill-shaped, white bg, strong shadow `0 1px 2px + 0 4px 12px`
- Divided into sections: Where / When / Who with vertical dividers
- Active section: white bg, elevated shadow
- Submit: `#FF385C` circle button with search icon, white icon

### Listing cards
- No border, no outer shadow
- Image: 16:9 ratio, `border-radius: 12px`, covers full width
- Below image: title (weight 600) + subtitle (grey) + price per night
- Hover: image scales 1.04 subtly
- Favorite heart: absolute top-right, white icon, on hover fills red
- Pagination: loads more on scroll

### Buttons
- Primary: `#FF385C` bg, white text, `border-radius: 8px`, 14px 24px
- Secondary: white bg, `#222` border, same radius
- Large (booking): full-width, 48px height, gradient `#E61E4D → #E31C5F → #D70466`
- Ghost: no border, text only, underline on hover

### Filters bar
- Horizontal scroll pill buttons: `border: 1px solid #DDDDDD`, `border-radius: 9999px`
- Active: `#222222` bg, white text
- Filters modal: full-screen on mobile, panel on desktop

### Rating
- Star: `#FF385C` filled star (not yellow)
- Score: bold 14px + `·` separator + review count link
- Superhost badge: `#FF5A5F` star icon + "Superhost" label

### Date picker
- Calendar: flat design, `#222` for selected, range highlight `#F7F7F7`
- Selected date circle: `#222222` bg, white text
- Today: underline

### Booking card
- Sticky sidebar card, `border: 1px solid #DDDDDD`, `border-radius: 12px`
- Shadow: `0 6px 16px rgba(0,0,0,0.12)`
- Price: large 22px, bold, `/night` in smaller weight

## Visual Patterns
- **Photography-first**: large, beautiful listing images — design frames them
- **Category icons**: small grayscale custom icons (beach, mountains, etc.)
- **Map integration**: always paired with listings — map is core UI
- **Trust signals**: verified host badge, Superhost, ratings prominent
- **Review cards**: 2-col grid, truncated with "Show more"
- **Host avatar**: circular, 56px, with Superhost ring when applicable

## Motion
- Duration: 150–250ms
- Listing image: scale on hover (1.04, ease-out)
- Search bar expand: smooth width + shadow transition
- Map markers: bounce in on new results
- Photo carousel: swipe/drag, smooth inertia
