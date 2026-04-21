# GitHub Design Language

## Aesthetic
Utilitarian, trusted, developer-native. Light mode default with full dark mode parity (GitHub Dark). Data-dense but readable. Primer Design System. Muted blue links, green success, red danger — familiar conventions respected.

## Color Usage
- **Light canvas**: `#FFFFFF` default, `#F6F8FA` subtle, `#F0F2F4` inset
- **Dark canvas**: `#0D1117` default, `#161B22` subtle
- **Text (light)**: `#1F2328` primary, `#656D76` secondary
- **Text (dark)**: `#E6EDF3` primary, `#848D97` secondary
- **Link**: `#0969DA` — always underline on hover
- **Border (light)**: `#D0D7DE`, muted `#D8DEE4`
- **Border (dark)**: `#30363D`
- **Accent**: `#0969DA` (blue) — buttons, focus, links
- **Success**: `#1A7F37` text, `#DAFBE1` bg
- **Danger**: `#CF222E` text, `#FFEBE9` bg
- **Attention**: `#9A6700` text, `#FFF8C5` bg
- **Done**: `#8250DF` text, `#FBEFFF` bg (purple for merged/done)
- **Diff add**: `#D1F8D9` bg; **diff remove**: `#FFCECB` bg

## Typography
- Font: system stack (`-apple-system, BlinkMacSystemFont, "Segoe UI", "Noto Sans", Arial`)
- Mono: `SFMono-Regular, Consolas, Liberation Mono, Menlo`
- Body: 14px, weight 400, line-height 1.5
- H1: 32px bold; H2: 24px bold; H3: 20px semibold
- Small: 12px for metadata, timestamps, labels
- Code inline: 85% font size, `#F6F8FA` bg, 3px radius, 0.2em padding

## Spacing
4px base. Content max-width: 1012px. Repo page layout uses 12-column grid. Component internal padding: 8–16px. Page header: 16px padding.

## Layout
- **Repository page**: header + tab nav + main content (2/3) + sidebar (1/3)
- **Feed**: centered single column, 768px max
- **Issues/PRs list**: full-width list with filters sidebar
- **Code view**: file tree sidebar (260px) + code panel

## Components

### Buttons
- Primary: `#1F883D` bg (green), white text, `border-radius: 6px`
- Default: white bg, `#1F2328` text, `border: 1px solid rgba(31,35,40,0.15)`
- Danger: `#CF222E` bg on confirm
- Height: 32px, padding: 5px 16px
- Inset shadow: `inset 0 1px 0 rgba(255,255,255,0.25)`
- Active: pressed shadow

### Labels (issue labels)
- `border-radius: 9999px`, 12px 8px padding, 12px font
- Any hex bg, auto contrast text (light or dark)
- Default set: bug (red), enhancement (blue), question (pink)

### Cards / Boxes
- `border: 1px solid #D0D7DE`, `border-radius: 6px`
- No shadow by default — flat design
- Header: `#F6F8FA` bg with bottom border

### Navigation tabs
- `border-bottom: 1px solid #D0D7DE` underline
- Active tab: `border-bottom: 2px solid #FD8C73` (orange/salmon highlight)
- Tab items: 15px text, 8px 16px padding

### Avatar
- Circular, sizes: 16/20/24/32/40px
- Default: gray placeholder with GitHub silhouette

### Code review diff
- Line numbers: `#6E7781`, 1px border right
- Add line: `#CCFFD8` bg (light), gutter `#C6E6CD`
- Remove line: `#FFD7D5` bg, gutter `#F5BFBB`
- Monospace 12px, line-height 20px

### Status indicators
- Issue open: green circle outline
- Issue closed: purple filled circle
- PR open: green icon; merged: purple; draft: gray; closed: red

## Visual Patterns
- **Octicons** icon set — 16px default, 24px for empty states
- **Repository cards** on profile: border box, language dot + color
- **Contribution graph** (heatmap): 13px squares, 4 green intensity levels
- **Markdown rendering**: full GFM with tables, task lists, syntax highlighting
- **@mentions / #references**: blue links inline in text
- **Timeline events**: left-aligned vertical line, icons on dots

## Motion
- Minimal — mostly instant transitions
- Dropdown: 100ms fade in
- Tooltips: 300ms delay, 150ms fade
- No decorative animations
