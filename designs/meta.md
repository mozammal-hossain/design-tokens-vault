# Meta (Facebook) Design Language

## Aesthetic
Social, accessible, familiar. Light gray backgrounds with white card surfaces. Facebook blue `#0866FF` is the primary interactive color. Optimistic typeface. Designed for universal accessibility across billions of users globally. Information-dense but readable.

## Color Usage
- **Light bg**: `#F0F2F5` (blue-gray tint)
- **Dark bg**: `#18191A`
- **Card surface (light)**: `#FFFFFF`
- **Card surface (dark)**: `#242526`
- **Surface hover (light)**: `#E4E6EB`
- **Surface hover (dark)**: `#3A3B3C`
- **Text (light)**: `#050505`
- **Text (dark)**: `#E4E6EB`
- **Secondary text (light)**: `#65676B`
- **Secondary text (dark)**: `#B0B3B8`
- **Disabled**: `#BCC0C4`
- **Links**: `#0866FF`
- **Brand**: `#0866FF` (Facebook blue)
- **Border (light)**: `#CED0D4`
- **Border (dark)**: `#393A3B`
- **Messenger**: `#0084FF`; Instagram: `#E1306C`; WhatsApp: `#25D366`
- **Reactions**: like blue, love red, haha yellow, wow yellow, sad yellow, angry orange

## Typography
- Font: **Optimistic Display** (headings), **Optimistic Text** (body)
- Fallback: Helvetica, Arial
- Feed post text: 15px, weight 400, line-height 1.3333
- Username/name: 15px, weight 700
- Comment text: 15px, weight 400
- Timestamp: 12–13px, `#65676B`
- Navigation labels: 12px
- Profile name large: 20px, weight 700

## Spacing
4px base. Feed posts: 12px padding. Card inner: 12–16px. Avatar gaps: 8px. Action button row: 12px vertical padding. Story circle gap: 8px.

## Layout
- **Desktop 3-column**:
  - Left: navigation sidebar (280px)
  - Center: feed (500px max)
  - Right: contacts/suggestions sidebar (280px)
- **Header**: fixed, full-width, 56px, white
  - Logo left, search bar, nav icons center, profile/notifications right
- **Mobile**: bottom tab bar, full-screen feed

## Components

### Post card
- `background: #FFFFFF`, `border: 1px solid #CED0D4`, `border-radius: 8px`
- Shadow: `0 2px 12px rgba(0,0,0,0.12)`
- Header: avatar (40px) + name + privacy indicator + timestamp + more menu
- Content: text + link preview or photo/video
- Reactions bar: reaction counts row
- Action buttons: Like / Comment / Share (full width, 3 columns)
- Divider: 1px above actions

### Like button
- Thumb icon + "Like" text, `#65676B` default
- Liked state: `#0866FF` color, filled thumb
- Long-press/hover: reaction emoji picker floats above

### Reactions picker
- Horizontal row of emoji, scale 1→1.5 on hover with name label
- 6 reactions: 👍❤️😆😮😢😠
- `border-radius: 9999px` container, white bg, shadow

### Stories
- Circular thumbnails, 56px, with gradient ring (unviewed)
- Gradient: brand blue ring
- Viewed: gray ring
- User avatar inside circle, name below (11px)

### Navigation (left sidebar)
- Profile shortcut at top
- Items: 36px height, `border-radius: 8px`
- Active: `#E7F3FF` bg, `#0866FF` icon
- Hover: `#E4E6EB`
- Icons: 20px, colored for each section

### Buttons
- Primary: `#0866FF` bg, white text, `border-radius: 6px`
- Secondary: `#E4E6EB` bg, `#050505` text
- Height: 36px, padding: 8px 12px, font: 15px weight 600

### Comment input
- Rounded input: `border-radius: 20px`, `#F0F2F5` bg
- Placeholder: "Write a comment..."
- Send icon appears when text entered

### Messenger bubble
- Primary: `#0084FF` bg, white text
- Received: `#F0F2F5` bg, dark text
- `border-radius: 18px` bubbles
- Time: centered between message groups

## Visual Patterns
- **Birthdays**: cake icon, separate module
- **Events**: illustrated card headers
- **Groups**: cover photo + member count
- **Marketplace**: product grid with image + price
- **Reels**: vertical full-screen video, TikTok-style

## Motion
- Like reaction: heart bounce animation
- Story ring: progress bar on viewing
- Feed load: skeleton shimmer `#E4E6EB` → `#F0F2F5`
- Photo expand: zoom + backdrop fade
- Dropdown menus: 150ms fade + scale
