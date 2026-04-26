# Design System Inspiration of Grab

## 1. Visual Theme & Atmosphere

Grab's design is a mobile-first, super-app system built around speed, trust, and clarity. The interface centers on Grab Green (#00B14F) — a vibrant, energetic green that signals reliability and forward motion. Against clean white backgrounds, this green creates strong CTAs while maintaining a friendly, approachable character.

The design uses generous border radius (pill-shaped buttons at 100px, 16px cards) that feels modern and approachable — reflecting Grab's position as Southeast Asia's everyday app for rides, food, payments, and more. Typography is set in Inter, a clean geometric sans-serif that renders clearly at all sizes on mobile screens.

**Key Characteristics:**
- Grab Green (#00B14F) as the single dominant brand color
- Pill-shaped buttons (100px radius) — approachable, mobile-optimized
- Inter — clean geometric sans-serif, excellent mobile legibility
- Surface inputs (background-colored, border appears on focus only)
- Service chips for app navigation (GrabCar, GrabFood, GrabPay)
- Dark mode: green brightens to #00C957 for contrast on dark surfaces

## 2. Color Palette & Roles

### Brand
- **Grab Green** (`#00B14F`): Primary — buttons, links, active states
- **Green Dark** (`#007A36`): Pressed/hover state
- **Green Mid** (`#00994A`): Active/selected state
- **Green Light** (`#E6F7EE`): Tonal surface for ghost buttons and chips

### Surface & Text
- **Near Black** (`#1A1A1A`): Primary text
- **Secondary** (`#6B6B6B`): Supporting text, metadata
- **Surface** (`#F5F5F5`): Input and secondary backgrounds
- **Border** (`#E0E0E0`): Dividers
- **Error** (`#E53935`): Error state

### Dark Mode
- Background: `#121212`, Surface: `#1E1E1E`
- Text: `#E8E8E8`, Secondary: `#9A9A9A`
- Green brightens to `#00C957` for legibility

## 3. Typography

**Typeface:** Inter (Google Fonts)

| Role    | Size | Weight | Notes              |
|---------|------|--------|--------------------|
| Heading | 28px | 700    | -0.3px tracking    |
| Title   | 22px | 700    | -0.3px tracking    |
| Section | 16px | 600    | UI section headers |
| Body    | 14px | 400    | Primary reading    |
| Label   | 12px | 500    | Metadata, ETA      |
| Caption | 11px | 400    | Driver/car info    |

## 4. Components

### Buttons
- **Primary**: Grab Green bg, white text, 100px pill radius
- **Outlined**: transparent bg, green text, 2px green border, 100px radius
- **Ghost (Tonal)**: green-light bg, green text, 100px radius
- **FAB**: circular, green bg, used for primary action

### Cards
- Border radius: 16px
- Shadow: `0 2px 8px rgba(0,0,0,0.08)`
- No border — shadow defines card edges

### Forms
- Surface-colored background (no border in default state)
- 2px green border on focus
- 12px border radius (softer than typical)

## 5. Spacing & Layout

8px base grid. Common values: 4, 8, 12, 16, 24, 32px.

## 6. Border Radius

| Value  | Usage          |
|--------|----------------|
| 8px    | Small elements |
| 12px   | Inputs         |
| 16px   | Cards          |
| 24px   | Large sections |
| 100px  | Buttons (pill) |
| 50%    | Avatars        |
