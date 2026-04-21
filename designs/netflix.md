# Netflix Design Language

## Aesthetic
Dark, cinematic, content-first. Pure `#141414` background lets colorful thumbnails pop. Red brand is used sparingly — only for CTAs and logo. Everything serves the content: rows of cards, large hero imagery, bold overlays. Feels like a premium streaming theater.

## Color Usage
- **App bg**: `#141414`
- **Elevated bg**: `#181818`
- **Card surface**: `#2F2F2F`
- **Card hover**: `#3D3D3D`
- **Header**: `rgba(20,20,20,0.95)` (slightly transparent when over content)
- **Text primary**: `#FFFFFF`
- **Text secondary**: `#B3B3B3`
- **Text muted**: `#737373`
- **Brand red**: `#E50914`
- **Brand red hover**: `#B20710`
- **Match %**: `#46D369` (green — high match indicator)
- **New badge**: `#46D369`
- **Border**: `#404040` (rare)

## Typography
- Font: **Netflix Sans** (fallback: Helvetica Neue, Arial)
- Hero title: 48–72px, weight 700, text-shadow for readability on images
- Row section headers: 20–24px, weight 700
- Card metadata: 12–13px, `#B3B3B3`
- Buttons: 16px, weight 700
- Body/modals: 16px, weight 400, line-height 1.5
- Timestamps/durations: monospace, `#B3B3B3`

## Spacing
4px base. Row cards: 4px gap between cards. Row label: 20px padding bottom. Section rows: 32–48px vertical gap. Hero: full viewport height. Card hover expands — extra padding absorbed by scale transform.

## Layout
- **Full-width app**: no max-width constraint — fills viewport
- **Header**: fixed, transparent → `rgba(20,20,20,0.95)` on scroll
- **Hero billboard**: 100vh height, left-bottom content overlay
- **Content rows**: horizontal scroll, labeled sections
- **Profile selector**: centered grid on profile page

## Components

### Hero billboard
- Full viewport height, background image/video
- Left-bottom-aligned title + metadata + buttons
- Title: large bold, text-shadow
- Two buttons: "Play" (white bg) + "More Info" (`rgba(109,109,110,0.7)` bg)
- Top fade gradient: `linear-gradient(to bottom, rgba(20,20,20,0.5) 0%, transparent)`
- Bottom fade: `linear-gradient(to top, #141414 10%, transparent)`

### Content rows
- Label: 20px bold white, hover shows "Explore All ›" link
- Cards: horizontal overflow-x scroll, hidden scrollbar
- Peek: partial next card visible at row edge
- Row padding: 4% horizontal (responsive)

### Cards
- Aspect: 16:9 (movie thumbnails)
- `border-radius: 4px`
- Normal: flat, no border, no shadow
- Hover: scale 1.05, shadow, expand to 1.15 at center
- Expanded hover card (after 500ms delay): shows title, metadata, action buttons, badges
- Expanded card: `border-radius: 4px`, `#181818` bg below image

### Expanded hover card
- Same image, larger
- Below image: row of action icons (play, add, like, dislike, chevron)
- Badge row: Match %, maturity rating, episode count/duration
- Genre tags: small pills

### Buttons
- Play: white bg, `#000000` text, `border-radius: 4px`, 16px font weight 700
- Info: `rgba(109,109,110,0.7)` bg, white text, same
- Height: 42px, padding: 8px 24px
- Focus: white outline

### Episode list
- Numbered rows, 80px thumbnail left
- Episode title + duration right
- Description below in `#B3B3B3`
- Divider: 1px `#404040`

### Profile cards
- Circular avatar (80px)
- Name below: 16px `#E5E5E5`, hover `#FFFFFF`
- Add profile: dashed border circle
- Edit mode: lock icon overlay

### Progress bar
- Video scrubber: red track, white dot
- Episode progress on card: thin red bar at bottom edge of thumbnail

## Visual Patterns
- **N-Up grids** for Top 10: numbered oversized text overlapping cards
- **Continue watching row**: progress bar on each card thumbnail
- **Match percentage**: `#46D369` green with thumbs-up icon
- **Maturity ratings**: small bordered pill (TV-MA, PG-13, etc.)
- **Download badge**: phone icon on downloadable titles
- **Language selection**: globe icon, minimal dropdown

## Motion
- Card hover expand: 500ms delay trigger, scale 200ms ease
- Row scroll: smooth native scroll
- Hero background: subtle slow Ken Burns pan on still images
- Transition to playback: fade to black, then content
