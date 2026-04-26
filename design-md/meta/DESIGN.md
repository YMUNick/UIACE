# Design System Inspiration of Meta

## 1. Visual Theme & Atmosphere

Meta's design is a social-first system built around connection, community, and accessibility. The interface uses a light neutral surface (#F0F2F5) as the primary canvas — warm and familiar, reducing eye strain for extended use. The brand accent is Facebook Blue (#0866FF), appearing in primary buttons, links, and interactive highlights. Dark mode uses deep charcoal (#18191A) with elevated surfaces (#242526, #3A3B3C).

The design is intentionally approachable — moderate border radii (6px for buttons, 8–12px for cards), comfortable spacing, and a strong hierarchy that prioritizes content and interactions. The iconic reaction system and comment threads define the visual rhythm of the product.

**Key Characteristics:**
- Facebook Blue (#0866FF) as the primary accent on neutral (#F0F2F5) surface
- Conversational card UI — post composer, reaction bar, comment thread
- 6px button radius, 12px card radius — friendly and approachable
- Roboto / system-ui for legible, accessible body text
- Elevated surface system for dark mode (layered grays)
- Pill-shaped tags and reaction badges

## 2. Color Palette & Roles

### Brand
- **Facebook Blue** (`#0866FF`): Primary buttons, links, active states
- **Blue Dark** (`#0052CC`): Pressed/hover state
- **Blue Light** (`#E7F3FF`): Tinted backgrounds, selection highlights

### Surface & Text
- **Background** (`#F0F2F5`): Page canvas
- **Surface** (`#FFFFFF`): Card background
- **Surface 2** (`#F7F8FA`): Subtle secondary panels
- **Border** (`#CED0D4`): Dividers and input borders
- **On Background** (`#1C1E21`): Primary text
- **Secondary** (`#65676B`): Metadata, labels, timestamps

### Dark Mode
- Background: `#18191A`, Surface: `#242526`, Surface 2: `#3A3B3C`
- Text: `#E4E6EB`, Secondary: `#B0B3B8`
- Blue accent: `#2D88FF`

### Semantic
- **Error** (`#F02849`): Destructive, alerts
- **Success** (`#42B72A`): Confirmations, online indicator
- **Warning** (`#F7B928`): Caution states

## 3. Typography

**Typeface:** Roboto / System UI fallback

| Role    | Size | Weight | Notes              |
|---------|------|--------|--------------------|
| Display | 24px | 700    | Page titles        |
| Title   | 18px | 600    | Post author, cards |
| Section | 15px | 600    | Section headers    |
| Body    | 15px | 400    | Post content       |
| Label   | 13px | 400    | Metadata, time     |
| Caption | 12px | 400    | Reaction counts    |

## 4. Components

### Buttons
- **Primary**: Blue bg, white text, 6px radius
- **Secondary**: White bg, gray border, dark text, 6px radius
- **Ghost**: Transparent, blue text, no border
- **Destructive**: Red bg or red text

### Cards (Post)
- Border radius: 12px — friendly, modern
- White surface with subtle shadow
- Composer bar at top with avatar + input
- Reaction bar: Like, Love, Haha, Wow, Sad, Angry

### Forms
- White bg, 1px #CED0D4 border, 6px radius
- Focus: 2px blue outline
- Error: red border + message below

## 5. Spacing & Layout

8px base grid. Cards use 16px internal padding. Feed has max-width 680px centered. Sidebars at 360px. Comment threads indented 32px.

## 6. Border Radius

| Value | Usage                  |
|-------|------------------------|
| 4px   | Small tags, badges     |
| 6px   | Buttons, inputs        |
| 12px  | Cards, modals          |
| 50%   | Avatars, reaction icons|

## 7. Elevation / Shadow

| Level | Usage                   | Shadow                              |
|-------|-------------------------|-------------------------------------|
| 0     | Background              | none                                |
| 1     | Cards                   | `0 1px 2px rgba(0,0,0,0.1)`        |
| 2     | Dropdowns, popovers     | `0 4px 12px rgba(0,0,0,0.15)`      |
| 3     | Modals, dialogs         | `0 8px 24px rgba(0,0,0,0.2)`       |
