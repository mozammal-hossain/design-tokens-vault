# X (Twitter) Design Language

## Aesthetic
Minimal, text-first social media. White/black depending on mode — no intermediate colors. Clean feed of posts. Black brand (since rebrand to X). Blue (legacy Twitter blue) remains for interactive states. Every element stripped to its essence. Feels editorial.

## Color Usage
- **Light bg**: `#FFFFFF`
- **Dark bg**: `#000000`
- **Dim bg**: `#15202B` (alternative dark)
- **Surface (light)**: `#F7F9F9`
- **Surface (dark)**: `#16181C`
- **Hover (light)**: `rgba(0,0,0,0.03)`
- **Hover (dark)**: `rgba(255,255,255,0.03)`
- **Text (light)**: `#0F1419`
- **Text (dark)**: `#E7E9EA`
- **Secondary (light)**: `#536471`
- **Secondary (dark)**: `#71767B`
- **Links**: `#1D9BF0` (Twitter blue, retained)
- **Border (light)**: `#EFF3F4`
- **Border (dark)**: `#2F3336`
- **Verified gold**: `#FFD400`
- **Like**: `#F91880` (pink)
- **Repost**: `#00BA7C` (green)
- **Error**: `#F4212E`

## Typography
- Font: system stack (`-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto`)
- Tweet text: 15–17px, weight 400, line-height 1.3125
- Username (@handle): 15px, weight 400, `#536471`
- Display name: 15px, weight 700
- Trending topic: 15px, weight 700
- Count labels: 13–15px, `#536471`
- Timestamps: 15px, `#536471`
- CTA buttons: 15px, weight 700

## Spacing
4px base. Tweet cells: 16px padding. Timeline dividers: 1px `#EFF3F4`. Bottom tab bar (mobile): 52px. Left nav (desktop): 275px.

## Layout
- **Desktop 3-column**:
  - Left nav: 275px (flex content, logo top)
  - Feed: 600px
  - Right sidebar: 350px (search, trends, suggestions)
- **Header (mobile)**: minimal, avatar left, X logo center
- **Bottom nav (mobile)**: Home / Search / Notifications / Messages

## Components

### Tweet
- Avatar: 40px circle, left-aligned
- Header row: display name (bold) + @handle + `·` + timestamp
- Content: text (up to 280 chars), media, poll, card
- Action row: Reply / Repost / Like / Bookmark / Share
  - Each: icon + count, `#536471` default
  - Like: hover/active → `#F91880` + filled heart
  - Repost: hover/active → `#00BA7C` + filled arrows
  - All: hover shows colored bg circle behind icon
- `border-bottom: 1px solid #EFF3F4`

### Tweet media
- Images: `border-radius: 16px`, 4-grid max
- Video: same radius, play overlay
- Card (link preview): `border: 1px solid #EFF3F4`, `border-radius: 16px`, image + site name + title

### Compose box
- Avatar left + multi-line text area right
- Placeholder: "What is happening?!"
- Bottom bar: media buttons + emoji + poll + schedule + location | char counter + post button
- Post button: `#000000` bg, white text (or blue if following old style), `border-radius: 9999px`
- Width: 584px max

### Buttons
- Primary (Follow): outline style — `border: 1px solid #0F1419`, `border-radius: 9999px`, black bg on hover
- Following state: "Following" outline → hover "Unfollow" red destructive
- CTA (Post): `#000000` bg, white text, pill shape
- Height: 32–36px

### Left navigation
- X logo: 32px, top
- Items: 68px height, icon (26px) + label
- Active: weight 700 text
- Hover: `rgba(15,20,25,0.1)` bg, `border-radius: 9999px`
- Post button: large black pill, 52px height, full label

### Right sidebar
- Search bar: `#EFF3F4` bg, `border-radius: 9999px`, 44px height
- Trends card: `border-radius: 16px`, `#F7F9F9` bg
- Trend row: category + topic (bold) + tweet count
- Who to follow card: same card style, avatar + name + follow button

### Notifications
- Each: icon (reply/like/repost/follow) colored + content
- Grouped: multiple people, stacked avatars

## Visual Patterns
- **Verified checkmarks**: blue (official), gold (subscribed), gray (government)
- **Thread view**: vertical connecting line between tweets
- **Quote tweet**: nested card inside tweet
- **Poll**: percentage bars, `border-radius: 4px`, brand blue fill
- **Spaces**: purple gradient audio room indicator
- **Community notes**: yellow warning strip under misleading content

## Motion
- Like animation: heart burst (pink particles, 200ms)
- Repost: green color swap (150ms)
- Pull to refresh: X logo spins
- Media open: scale up from card to full-screen (200ms)
