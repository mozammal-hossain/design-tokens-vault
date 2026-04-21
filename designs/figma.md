# Figma Design Language

## Aesthetic
Design-tool precision. Dark editor panels contrast with bright canvas. Clean Inter UI chrome at 12–14px. Five-color brand (the Figma component colors). Functional density — every pixel in the panel serves a purpose. Light mode for marketing, dark for the tool itself.

## Color Usage
- **Editor bg**: `#1E1E1E` (canvas surround)
- **Toolbar/panels**: `#2C2C2C`
- **Panel surface**: `#2C2C2C`, section bg `#383838`
- **Canvas**: `#F5F5F5` default
- **Light bg (marketing)**: `#FFFFFF`
- **Surface light**: `#F5F5F5`
- **Text (editor)**: `#FFFFFF` primary, `#B3B3B3` secondary
- **Text (light)**: `#000000` primary, `#666666` secondary
- **Border (editor)**: `#3D3D3D`
- **Brand green**: `#0ACF83` (primary CTA)
- **Brand blue**: `#1ABCFE`
- **Brand red**: `#FF7262`
- **Brand purple**: `#A259FF`
- **Brand orange**: `#F24E1E`
- **Selection blue**: `#18A0FB`

## Typography
- Font: **Inter**
- Panel labels: 11px, weight 400, `#B3B3B3`
- Input values: 11–12px, weight 400
- Section headers: 11px, weight 600, uppercase
- Marketing headings: 32–64px, weight 600–700
- Body: 14–16px, weight 400, line-height 1.5
- Mono: Roboto Mono 11px for raw values

## Spacing
4px base. Editor panels: 8px padding. Property rows: 28px height. Input pairs: side-by-side in 50% columns. Canvas: free-form, no grid constraint.

## Layout
- **Editor shell**:
  - Toolbar top: 40px, `#2C2C2C`
  - Left panel (layers/assets): 240px, `#2C2C2C`
  - Canvas: flex-fill, `#F5F5F5`
  - Right panel (design/prototype): 240px, `#2C2C2C`
- **Marketing**: centered, max 1100px

## Components

### Editor toolbar (top)
- File title center, back arrow left
- Move/frame/pen/text/shape/hand tools left section
- Zoom %, present, share, comment right section
- Height: 40px, bg `#2C2C2C`, separator `#3D3D3D`

### Layers panel
- Tree list, 24px row height
- Component icon: purple; frame: blue outline; group: gray brackets
- Indent: 12px per level
- Hover: `rgba(255,255,255,0.06)`
- Selected: `rgba(24,160,251,0.2)`
- Visibility/lock icons appear on hover at row right

### Design panel (right)
- Section separators: 1px `#3D3D3D` with section label
- Property rows: 28px, label left `#B3B3B3` + value input right
- Inputs: `border-radius: 2px`, `#3C3C3C` bg, no border until focus
- Focus: `#18A0FB` border
- Color swatch: 16px square with checkerboard bg, `border-radius: 2px`
- XYZ/WH values: 2-per-row in small paired inputs

### Inputs (editor)
- Height: 24px
- Font: 11px
- Bg: `#3C3C3C`
- Text: `#FFFFFF`
- Focus ring: `#18A0FB`
- Stepper arrows on hover

### Buttons (marketing/community)
- Primary: `#0ACF83` bg, white text, `border-radius: 6px`
- Secondary: outlined, same radius
- Height: 40px, padding: 8px 24px

### Modals
- Dark panel `#2C2C2C` with border `#3D3D3D`
- `border-radius: 8px`
- Backdrop: `rgba(0,0,0,0.5)`

### Color picker
- HSB square gradient
- Hue slider bar
- Opacity slider bar
- Hex/RGB/HSL/HSB toggles
- Eyedropper button

## Visual Patterns
- **Selection handles**: blue squares at corners/edges, 8px
- **Guides/rulers**: teal lines, draggable from ruler edge
- **Component badges**: purple `◆` icon for components
- **Auto layout**: orange/teal padding visualization on selection
- **Prototyping arrows**: purple connecting lines between frames
- **Community thumbnails**: card grid, cover art + author avatar

## Motion
- Canvas zoom/pan: immediate, no easing
- Panel collapse: 150ms ease
- Tooltip: 300ms delay, instant disappear
- Component swap: instant
