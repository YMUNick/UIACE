# Design System Inspiration of foodpanda

## 1. Visual Theme & Atmosphere

foodpanda's design is a vibrant, food-forward system built around appetite and urgency. The unmistakable Panda Pink (#D70F64) — a deep magenta — dominates the interface as the header background, primary CTA color, and brand accent. This bold, saturated pink creates strong emotional contrast against white content areas and immediately signals food, fun, and speed.

The design uses generous pill-shaped buttons (100px radius) and rounded cards (16px) that feel app-like and tactile, reflecting foodpanda's mobile-first delivery platform. Typography is set in Inter, providing clean legibility for restaurant names, ETA information, and menu items at varying sizes.

A notable design pattern is the pink navigation bar (not just a logo) — the full nav is Panda Pink, creating an immersive brand header that makes the brand unmissable.

**Key Characteristics:**
- Full-bleed pink (#D70F64) navigation bar — brand-first header
- Pill-shaped buttons (100px radius) — mobile-optimized, approachable
- Promotional badges (pill-shaped) on restaurant cards — urgency/offers
- Inter — clean geometric sans-serif, excellent mobile legibility
- Pink tonal light (#FCE4EF) for hero backgrounds and ghost buttons
- Dark mode: pink brightens to #F0257A, dark nav becomes #1A0B11

## 2. Color Palette & Roles

### Brand
- **Panda Pink** (`#D70F64`): Primary — nav bar, buttons, accents
- **Pink Dark** (`#B0094F`): Pressed/hover state
- **Pink Mid** (`#E91E7A`): Active/selected state
- **Pink Light** (`#FCE4EF`): Tonal surface for ghost buttons and hero bg

### Surface & Text
- **Near Black** (`#1A1A1A`): Primary text
- **Secondary** (`#666666`): Supporting text, metadata
- **Surface** (`#F5F5F5`): Input and secondary backgrounds
- **Border** (`#E0E0E0`): Dividers
- **Error** (`#D32F2F`): Error state

### Dark Mode
- Background: `#121212`, Surface: `#1E1E1E`, Nav: `#1A0B11`
- Text: `#E8E8E8`, Secondary: `#9A9A9A`
- Pink brightens to `#F0257A` for contrast on dark surfaces
- Tonal pink surface shifts to `#2E0A1C`

## 3. Typography

**Typeface:** Inter (Google Fonts)

| Role     | Size | Weight | Notes              |
|----------|------|--------|--------------------|
| Heading  | 28px | 700    | -0.3px tracking    |
| Title    | 22px | 700    | -0.3px tracking    |
| Section  | 16px | 600    | Category headers   |
| Body     | 14px | 400    | Descriptions       |
| Label    | 12px | 500    | ETA, distance      |
| Caption  | 11px | 400    | Fine print, fees   |

## 4. Components

### Buttons
- **Primary**: Panda Pink bg, white text, 100px pill radius
- **Outlined**: transparent bg, pink text, 2px pink border, 100px radius
- **Ghost (Tonal)**: pink-light bg, pink text, 100px radius
- **FAB**: circular, pink bg, used for "add to cart" action

### Cards (Restaurant)
- Border radius: 16px
- Shadow: `0 2px 8px rgba(0,0,0,0.08)`
- Promotional badge: pill-shaped (100px radius) on card image

### Forms
- Surface-colored background (no border in default state)
- 2px pink border on focus
- 12px border radius

## 5. Spacing & Layout

8px base grid. Common values: 4, 8, 12, 16, 24, 32px.

## 6. Border Radius

| Value  | Usage              |
|--------|--------------------|
| 8px    | Small elements     |
| 12px   | Inputs             |
| 16px   | Cards              |
| 24px   | Large sections     |
| 100px  | Buttons, badges    |
| 50%    | Avatars            |
