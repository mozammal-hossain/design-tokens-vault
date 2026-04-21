# Discord Design Language

## Aesthetic
Dark, layered, community-focused. Three-tone dark palette (tertiary darkest → secondary → primary). Blurple brand. Dense sidebar of servers and channels. Feels like a chat client evolved into a platform — heavy, feature-rich, yet familiar.

## Color Usage
- **Tertiary bg**: `#1E1F22` (darkest — server list bar)
- **Secondary bg**: `#2B2D31` (channel sidebar)
- **Primary bg**: `#313338` (main chat area)
- **Surface**: `#383A40` (input, cards)
- **Floating**: `#111214` (tooltips, menus)
- **Text normal**: `#DBDEE1`
- **Text muted**: `#80848E`
- **Text link**: `#00A8FC`
- **Brand blurple**: `#5865F2`
- **Brand hover**: `#4752C4`
- **Interactive normal**: `#B5BAC1`
- **Interactive hover**: `#DBDEE1`
- **Interactive active**: `#FFFFFF`
- **Status online**: `#23A55A`; idle: `#F0B132`; DND: `#F23F43`; offline: `#80848E`
- **Danger**: `#DA373C`; warning: `#F0B132`; positive: `#23A55A`
- **Nitro**: `#FF73FA`

## Typography
- Font: **gg sans** (Discord's custom font, fallback: Noto Sans, Helvetica)
- Mono: Consolas, Andale Mono
- Chat messages: 16px, weight 400, line-height 1.375
- Username: 16px, weight 500
- Channel names: 15px, weight 500
- Section headers: 11px, weight 700, uppercase, `#80848E`
- Timestamps: 11px, `#80848E`

## Spacing
4px base. Very dense — sidebar items 26px height. Chat messages: 0 padding between same-author messages, 17px gap between different authors. Server icons: 48px, 8px gap.

## Layout
- **4-column shell** (left to right):
  1. Server list bar: 72px wide, `#1E1F22`
  2. Channel sidebar: 240px, `#2B2D31`
  3. Main chat: flex-fill, `#313338`
  4. Member list: 240px (optional), `#2B2D31`
- All panels scroll independently
- Message input: fixed at bottom of chat area

## Components

### Server icons
- 48px circle (inactive) → `border-radius: 16px` (active, square pill)
- Transition on hover/active: circle → squircle shape morph
- Notification badge: red circle, absolute top-right, 16px
- Server folder: layered icon stack

### Channel sidebar
- Section headers: 11px uppercase, 700 weight, `#80848E`, with expand arrow
- Channel items: 26px height, 8px left indent per category
- Hover: `rgba(79,84,92,0.32)` bg, `border-radius: 4px`
- Active: `rgba(79,84,92,0.64)` bg, `#FFFFFF` text
- Icons: `#80848E` → `#DBDEE1` on hover

### Messages
- Avatar: 40px circle, left-aligned
- Username + timestamp on first message of group
- Subsequent messages: 40px indent, no avatar/name (grouped)
- Hover reveals timestamp right, action toolbar (emoji, reply, more)
- Reactions: `#313338` bg pill, `border-radius: 4px`, emoji + count
- Embeds: left colored bar + content block

### Message input
- `#383A40` bg, `border-radius: 8px`, no outer border
- Placeholder: `#4E5058`
- Attachment, emoji, GIF icons right side
- Height grows with content

### Buttons
- Primary: `#5865F2` bg, white text, `border-radius: 3px`
- Danger: `#DA373C` bg
- Ghost: transparent, text only
- Sizes: sm (20px), md (32px), lg (38px)

### Status indicators
- Always circular dot, bottom-right of avatar
- Sizes match avatar: 10px for 32px avatar, 16px for 48px
- Offline: gray with hollow center

### Badges
- Boost: purple/gold crown
- Verified: blue checkmark (servers)
- Staff/Nitro: special icons

## Visual Patterns
- **Server boosting**: purple gradient treatment when boosted
- **Activity cards**: game/app name in rich presence below username
- **Voice channel**: user avatars in a row, speaking indicator (green ring pulse)
- **Sticker/emoji picker**: scrollable grid, search at top, category tabs
- **Channel categories**: bold uppercase collapsible sections
- **Slash commands**: `/` trigger, autocomplete dropdown

## Motion
- Server icon morphing: circle ↔ squircle on focus/hover (150ms)
- Message appear: instant, no animation (performance priority)
- Popouts: 200ms fade + scale
- Modals: fade-in backdrop + slide-up panel
