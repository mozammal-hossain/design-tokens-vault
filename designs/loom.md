# Loom Design Language

## Aesthetic
Clean, video-first SaaS. Purple-indigo brand with white surfaces. Feels modern and slightly playful — not as austere as developer tools, not as casual as consumer apps. The record button is the hero of the UI. Warm neutral backgrounds.

## Color Usage
- **Light bg**: `#FFFFFF`
- **Dark bg**: `#1A1A2E`
- **Surface (light)**: `#F9F9F9`
- **Surface (dark)**: `#252540`
- **Text (light)**: `#111111`
- **Text (dark)**: `#FFFFFF`
- **Secondary (light)**: `#787878`
- **Secondary (dark)**: `#ABABAB`
- **Border (light)**: `#E5E5E5`
- **Border (dark)**: `#3A3A5C`
- **Brand**: `#625DF5` (purple-indigo)
- **Brand hover**: `#4F4AC4`
- **Brand secondary**: `#FF4C00` (orange-red — used for record button, error)
- **Record red**: `#FF0000`
- **Success**: `#00B341`
- **Camera frame**: `#625DF5`

## Typography
- Font: **Inter**
- Dashboard headings: 20–28px, weight 600
- Video titles: 16px, weight 600, truncated single-line
- Body: 16px, weight 400
- Metadata (duration, date): 13–14px, `#787878`
- Labels: 14px, weight 500

## Spacing
4px base. Dashboard: 24px grid gap. Video card: 12px below thumbnail. Top nav: 56px. Side nav: 240px. Page padding: 24–32px.

## Layout
- **Dashboard**: left sidebar (240px) + content grid
- **Video player page**: centered video (max 960px) + sidebar comments
- **Library**: responsive grid (3–4 cols), card-based

## Components

### Record button
- Circular, 56px, `#FF4C00` bg, white record icon (●)
- Hover: slightly larger (60px), brighter
- Recording state: pulsing red ring animation
- Recorder toolbar: dark pill with camera / screen / mic toggles

### Video thumbnail cards
- 16:9 aspect ratio
- `border-radius: 12px`
- Duration badge: bottom-right, dark pill `rgba(0,0,0,0.7)`, white text
- Hover: slight scale 1.02, play button overlay (white circle, 48px)
- Below: title (600 weight) + views + date + owner avatar

### Video player
- Controls bar: dark gradient overlay on video bottom
- Progress bar: `#625DF5` fill, white scrubber dot
- Time: monospace white
- Chapters: markers on progress bar
- Speed: 1x/1.5x/2x selector
- Comment icon on scrubber: yellow dot where comments exist

### Sidebar (left)
- `#FFFFFF` bg, 240px
- Workspace logo top
- Nav items: 36px height, 8px 12px padding, `border-radius: 8px`
- Active: `#625DF5` bg, white text
- Hover: `#F0F0FF` (light purple tint)
- Workspace switcher at bottom

### Buttons
- Primary: `#625DF5` bg, white text, `border-radius: 8px`
- Secondary: `#F9F9F9` bg, `#111111` text, `border: 1px solid #E5E5E5`
- Record: `#FF4C00` bg, white text
- Height: 40px, font: 14px weight 600

### Comment thread (video page)
- Time-stamped comments appear in sidebar
- Clicking comment jumps to timestamp
- Reaction bar: emoji reactions below each comment
- Comment form: flat input with avatar

### Sharing modal
- Copy link input: full-width, pill shaped
- Permission toggles: anyone with link / workspace only / specific people
- Embed code block

## Visual Patterns
- **Webcam bubble**: circular webcam overlay in corner during recording
- **Screen recording cursor trail**: highlighted click indicators
- **Trim editor**: waveform timeline with in/out handles
- **AI transcription**: timed text alongside video
- **GIF thumbnail**: animated preview on hover in library
- **Watch page**: branded URL, viewer count, CTA to sign up below video

## Motion
- Record button pulse: `box-shadow` radial pulse 1.5s loop
- Thumbnail hover: 150ms scale ease-out
- Sidebar: 200ms slide
- Video scrub: immediate visual update
- Comment dot: bounce-in on appear
