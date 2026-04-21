# Spotify Design Language

## Aesthetic
Dark, energetic, music-first. Deep charcoal backgrounds with electric green brand. Card-heavy grid layouts showing album art. Typography is bold and tightly tracked for impact. Feels like a premium streaming app — playful but focused.

## Color Usage
- **App bg**: `#121212` (deep charcoal, not pure black)
- **Elevated bg**: `#1A1A1A`
- **Card surface**: `#282828`
- **Card hover**: `#3E3E3E`
- **Text primary**: `#FFFFFF`
- **Text secondary**: `#B3B3B3`
- **Text subdued**: `#6A6A6A`
- **Brand green**: `#1DB954` (the Spotify green)
- **Brand hover**: `#1ED760` (lighter on hover)
- **Brand press**: `#169C46` (darker on press)
- **Error**: `#E91429`

## Typography
- Font: **Circular Sp** / Circular (fallback: Helvetica, Arial)
- Album/playlist titles: 14–16px, weight 700, single-line truncated
- Artist/subtitle: 14px, weight 400, `#B3B3B3`
- Section headers: 24px, weight 700
- Navigation: 13px, weight 700, uppercase with tracking
- Now-playing track: 14px bold (title), 12px regular (artist)
- Letter-spacing on large headings: `-0.04em`

## Spacing
4px base. Cards use zero internal padding — image fills card completely. Below card: 12px for text. Card grids: 16px gap. Left nav: 8px vertical padding per item. Player bar: 64px height.

## Layout
- **Left sidebar**: 232px, `#121212`, fixed
  - Navigation links top
  - Library section fills rest
- **Main content**: flex-fill, scrollable
  - Top nav bar: absolute, gradient fade from section color
- **Now-playing bar**: fixed bottom, full width, 90px height, `#181818`

## Components

### Navigation sidebar
- Links: 14px, weight 700, `#B3B3B3`, hover `#FFFFFF`
- Active: `#FFFFFF`
- Icons: 24px, inline left of label
- Library list items: 56px height with album art thumbnail

### Cards (Album / Playlist / Artist)
- `border-radius: 4px` for square art, `9999px` circle for artist
- `#282828` bg, hover `#3E3E3E` (smooth transition)
- Play button: absolute bottom-right corner of card, only shows on hover
  - Green circle `#1DB954`, white play icon, `border-radius: 50%`, 48px
  - Slides in from below with opacity + transform on hover
- Title: 14px weight 700, white, one line truncated
- Subtitle: 13px, `#B3B3B3`
- Padding below art: 12px 12px 24px

### Play button states
- Play: green circle, white triangle
- Pause: green circle, white bars
- Hover: brightens to `#1ED760`
- Active/press: darkens to `#169C46`

### Now-playing bar
- 3-column layout: track info | player controls | volume + extras
- Track info: 40px album art + title/artist
- Controls: prev/shuffle/play-pause/next/repeat icons centered
- Progress bar: `#535353` track, `#FFFFFF` progress, green dot on hover
- Volume slider: same style as progress bar
- Heart icon, queue icon, volume icon all `#B3B3B3` → hover `#FFFFFF`

### Buttons
- Primary: `#1DB954` bg, `#000000` text, `border-radius: 9999px`, weight 700
- Secondary: transparent, white border, white text, same radius
- Height: 32px (sm), 48px (lg)

### Context menu
- `#282828` bg, `border-radius: 4px`, shadow `0 16px 24px rgba(0,0,0,0.3)`
- Items: 40px height, 16px text, hover `#3E3E3E`
- Dividers: 1px `#3E3E3E`

## Visual Patterns
- **Dominant color extraction**: page gradient pulls from album art dominant color
- **Album art everywhere**: the UI is built around displaying album/playlist covers
- **Mosaic playlist covers**: 4-image 2×2 grid for auto-generated covers
- **Listening activity**: friends sidebar showing what they play
- **Podcast cards**: same grid treatment as music
- **Greenroom/Live**: separate brand treatment, rare

## Motion
- Card play button: slide up + fade in on card hover (150ms)
- Volume/progress: smooth scrub, instant visual response
- Page transitions: fade, 200ms
- Now-playing: crossfade between track art colors
