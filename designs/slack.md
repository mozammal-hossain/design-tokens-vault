# Slack Design Language

## Aesthetic
Warm, professional, communication-first. Dark purple sidebar paired with white content area — the signature Slack look. Lato font gives warmth. Feels corporate-friendly but not sterile. Four-color logo (red/yellow/green/blue) creates a playful identity.

## Color Usage
- **Sidebar bg**: `#3F0E40` (deep purple — the iconic Slack sidebar)
- **Sidebar hover**: `#350D36`
- **Sidebar active**: `#1164A3`
- **Content bg**: `#FFFFFF`
- **Surface**: `#F8F8F8`
- **Text primary**: `#1D1C1D`
- **Text secondary**: `#616061`
- **Sidebar text**: `#CFC3CF` (muted lavender)
- **Sidebar active text**: `#FFFFFF`
- **Text link**: `#1264A3`
- **Border**: `#DDDDDD`
- **Brand**: `#4A154B` (Slack aubergine)
- **Logo red**: `#E01E5A`; yellow: `#ECB22E`; green: `#2EB67D`; blue: `#36C5F0`
- **Mention badge**: `#E01E5A` (red)
- **Online**: `#2BAC76`

## Typography
- Font: **Lato** (fallback: system sans-serif)
- Message text: 15px, weight 400, line-height 1.46668
- Username: 15px, weight 900 (bold)
- Channel name in sidebar: 15px, weight 400
- Unread channel: weight 700
- Section headers: 13px, `#616061`, uppercase
- Timestamps: 12px, `#616061`

## Spacing
4px base. Sidebar items: 28px height, 16px horizontal padding. Messages: 20px vertical gap between groups. Channel padding: 20px horizontal.

## Layout
- **3-column shell**:
  1. Workspace switcher: 68px, `#1D1135` (optional multi-workspace)
  2. Sidebar: 260px, `#3F0E40`
  3. Content: flex-fill, white
- Message input: fixed bottom
- Threads: right panel slides in (360px), pushes content

## Components

### Sidebar
- Section headers: 13px, `#CFC3CF80` dimmed, uppercase, expandable
- Channel items: `#` prefix, 28px height, 16px padding
- Hover: `rgba(255,255,255,0.1)` bg, `border-radius: 6px`
- Active: `#1164A3` bg, `#FFFFFF` text
- Unread: bold white text, dot indicator
- DM items: avatar (24px circle) + name + status dot

### Messages
- Avatar: 36px circle
- Username: bold, colored (custom or default)
- Timestamp: right side, shows on hover
- Message text: 15px, full markdown support
- Reactions: pill buttons, `border-radius: 9999px`, emoji + count
- Hover toolbar: emoji, reply, more (appears top-right of message)
- Thread preview: "X replies · Last reply X ago" link below message

### Message input
- Rich text box, `border: 1px solid #DDDDDD`, `border-radius: 8px`
- Toolbar: Bold, Italic, Strikethrough, Link, Lists, Code, Blockquote
- Bottom: Emoji, GIF, mention, attach buttons left; Send right
- Height: grows with content, max ~50vh

### Buttons
- Primary: `#007A5A` (green), white text, `border-radius: 4px`
- Danger: `#E01E5A`
- Height: 36px, padding: 0 16px

### Badges (notification)
- Red circle `#E01E5A`, white bold number, `border-radius: 9999px`
- Sizes: small (16px for sidebar), large (20px for workspace icon)

### Status indicators
- Small colored dot (8px), bottom-right of avatar
- Online: `#2BAC76`; Away: yellow circle with clock; DND: red minus

### Channel header
- Channel name + hash icon, large, bold
- Topic/description below in smaller muted text
- Action icons right: Call, DMs, More

## Visual Patterns
- **Huddles**: audio-first, small floating AV bar
- **Canvas**: embedded rich document in channel
- **Workflow builder**: visual node-based automation
- **App shortcuts**: bottom of message input slash menu
- **Custom emoji**: `border-radius: 4px` on emoji images
- **Code blocks**: `#1D1C1D` bg (light), `border-radius: 4px`, Monaco mono

## Motion
- Sidebar items: instant (no animation)
- Message input send: quick scale-out
- Thread panel: 200ms slide-in from right
- Unread divider: animated pulse on first view
