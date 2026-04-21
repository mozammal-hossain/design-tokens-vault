# Google Design Language

## Aesthetic
Material Design 3 (Material You). Clean, light, approachable. Rounded corners everywhere. Subtle elevation via shadows (not borders). Color theming adapts dynamically. Both sparse (Search) and data-dense (Workspace) — same system, different densities.

## Color Usage
- **Search bg**: `#FFFFFF` with `#F8F9FA` hover inputs
- **Light surface**: `#FFFFFF`, subtle `#F8F9FA`
- **Dark bg**: `#202124`
- **Dark surface**: `#303134`
- **Text (light)**: `#202124`
- **Text (dark)**: `#E8EAED`
- **Secondary (light)**: `#5F6368`
- **Secondary (dark)**: `#9AA0A6`
- **Link (light)**: `#1A0DAB` (classic Google blue)
- **Link (dark)**: `#8AB4F8`
- **Visited**: `#681DA8`
- **Brand blue**: `#4285F4`; red: `#EA4335`; yellow: `#FBBC05`; green: `#34A853`
- **Border**: `#DADCE0` light, `#3C4043` dark
- **Focus**: `#1A73E8`
- **Error**: `#D93025`

## Typography
- Font: **Google Sans** (primary), **Roboto** (secondary/body), **Google Sans Display** (hero)
- Mono: Roboto Mono
- Search result title: 20px, weight 400, `#1A0DAB` (link color)
- Search URL: 14px, `#0D652D` (green)
- Search snippet: 14px, `#4D5156`
- UI labels: 14px, weight 500 (Google Sans)
- Card headings: 16–20px, weight 500
- Body: 14–16px, weight 400, line-height 1.75

## Spacing
4px base. Search box: 44px height. Results: 20px between results. Material components: 8px internal padding minimum. Touch targets: minimum 48px.

## Layout
- **Search page**: single centered column, 652px max, logo + search box + results
- **Workspace (Docs/Sheets)**: toolbar top + document content
- **Google Home**: centered search bar, quick links grid
- **Material app layout**: top app bar + navigation rail (desktop) or bottom nav (mobile)

## Components

### Search bar
- `border: 1px solid #DADCE0`, `border-radius: 24px`, 44px height
- Hover: shadow `0 1px 6px rgba(32,33,36,0.28)`, border transparent
- Focus: same hover shadow
- Mic icon right, search icon left
- Google Lens icon (camera) right of mic
- Width: 584px max on search page

### Search results
- Title: 20px, `#1A0DAB`, no underline, hover underline
- URL: 13px, `#0D652D`
- Favicon: 16px circle left of URL
- Snippet: 14px, `#4D5156`, line-height 1.58
- Spacing between results: 20px
- Featured snippet: outlined box, `border-radius: 8px`, `#4285F4` left border

### Material buttons
- Filled: `#1A73E8` bg, white text, `border-radius: 20px`, 40px height
- Outlined: white bg, `#1A73E8` border + text
- Text: transparent bg, `#1A73E8` text
- Icon button: 40px circle, transparent bg, hover `rgba(26,115,232,0.08)`
- FAB: 56px circle, shadow elevation 3

### Cards (Material)
- `border-radius: 12px`, shadow elevation 1
- Hover: elevation 2 shadow
- No explicit border
- Padding: 16px

### Chips
- `border-radius: 8px`, `border: 1px solid #DADCE0`, 32px height
- 12px 16px padding, 14px text
- Selected: filled `#1A73E8` bg, white text, no border
- Hover: `#F1F3F4` bg

### Navigation (Workspace)
- Top bar: 64px, white, 1px bottom border
- Logo left, search center (wide), actions/avatar right
- Side drawer: 256px, rounded nav items `border-radius: 0 24px 24px 0`
- Active item: `#E8F0FE` bg, `#1A73E8` text

### Inputs (Workspace / Forms)
- Outlined style: `border-radius: 4px`, label floats up on focus
- Focus: `#1A73E8` 2px border
- Error: `#D93025` border, helper text below

## Visual Patterns
- **Material elevation**: shadows encode depth (0–5 scale)
- **Dynamic color**: M3 tonal palette shifts with user wallpaper on Android
- **Ripple effects**: click feedback on all interactive elements
- **Google Doodles**: homepage logo changes for events
- **Knowledge panels**: right sidebar cards with entity info
- **Search chips**: horizontal scroll filters below search bar

## Motion
- Material motion: standard `cubic-bezier(0.2, 0, 0, 1)` for most transitions
- Shared element transitions between views
- Ripple: radial expand from touch point, 300ms
- Container transform: element expands to fill new view
