# Design System Inspiration of Google

## 1. Visual Theme & Atmosphere

Google's design language — Material Design 3 (Material You) — is clean, adaptive, and built around dynamic color. The interface uses a pure white (#FFFFFF) canvas with cool neutral surfaces (#F8F9FA) and Google's four iconic brand colors: Blue (#4285F4), Red (#EA4335), Yellow (#FBBC05), and Green (#34A853). These four colors appear in the logo and punctuate UI accents, but the dominant interactive color is Google Blue.

Typography is set in Roboto — a humanist geometric sans-serif that balances warmth with technical precision. Roboto's wide character set and legibility at small sizes made it the default for Android and the broader Google ecosystem. Weight usage is restrained: 400 for body, 500 for labels and titles, 700 for bold emphasis.

Material Design 3 introduces tonal elevation — surfaces that get lighter as they rise higher — and a dynamic color system that can derive an entire palette from a single seed color.

**Key Characteristics:**
- Four-color brand logo system (blue, red, yellow, green)
- Roboto — geometric humanist sans-serif at all sizes
- Tonal elevation: surfaces lighten with altitude
- 8px spacing grid — consistent density across products
- Border radius scale: 4px → 8px → 12px → 16px → 28px
- Blue focus rings (rgba 40%) — consistent keyboard navigation affordance
- Material You dynamic color: seed → full tonal palette

## 2. Color Palette & Roles

### Brand
- **Google Blue** (`#4285F4`): Primary interactive color, buttons, links, focus ring
- **Google Red** (`#EA4335`): Brand accent, error states, logo letter
- **Google Yellow** (`#FBBC05`): Brand accent, warning states, logo letter
- **Google Green** (`#34A853`): Brand accent, success states, logo letter

### Surface & Text
- **On Background** (`#202124`): Primary text — cool dark, not pure black
- **Secondary** (`#5F6368`): Supporting text, labels, metadata
- **Surface** (`#F8F9FA`): Default page background
- **Surface 2** (`#F1F3F4`): Slightly darker tonal surface
- **Border** (`#DADCE0`): Dividers, input borders, outlined components
- **Blue Container** (`#E8F0FE`): Tonal surface for blue-accented components
- **Error** (`#D93025`): Error text and destructive state

### Dark Mode
- Background: `#202124`, Surface: `#2D2E31`
- Text: `#E8EAED`, Secondary: `#9AA0A6`
- Blue shifts to `#8AB4F8`, Red to `#F28B82`, Yellow to `#FDD663`, Green to `#81C995`

## 3. Typography

**Typeface:** Roboto (Google Fonts)

| Role      | Size | Weight | Notes              |
|-----------|------|--------|--------------------|
| Display   | 28px | 400    | Light, open        |
| Headline  | 22px | 500    | Medium emphasis    |
| Title     | 16px | 500    | UI section headers |
| Body      | 14px | 400    | Primary reading    |
| Label     | 12px | 500    | Caps, ls 0.4px     |
| Caption   | 11px | 400    | Metadata, hints    |

## 4. Components

### Buttons
- **Filled**: `#4285F4` bg, white text, 4px radius — primary actions
- **Outlined**: transparent bg, blue text, `#DADCE0` border — secondary actions
- **Text**: no border/bg, blue text, hover tonal bg — tertiary/inline actions
- **Icon**: circular tonal bg (`#E8F0FE`), 50% radius
- **Chip**: pill shape (20px radius), surface bg, border — filter/selection

### Cards
- Border radius: 8px
- Elevation Level 1 default: `0 1px 3px rgba(60,64,67,0.30), 0 1px 2px rgba(60,64,67,0.15)`
- Elevation Level 2 (hover): `0 2px 6px 2px rgba(60,64,67,0.15), 0 1px 2px rgba(60,64,67,0.30)`

### Forms
- 4px radius inputs, 1px `#DADCE0` border
- Focus: `#4285F4` border + `rgba(66,133,244,0.2)` 2px ring
- Error: `#D93025` border

## 5. Spacing & Layout

8px base grid. Common values: 4, 8, 12, 16, 24, 32px.

## 6. Border Radius

| Value | Usage              |
|-------|--------------------|
| 4px   | Inputs, small tags |
| 8px   | Cards, dialogs     |
| 12px  | Medium containers  |
| 16px  | Large containers   |
| 28px  | Full / pill shape  |
| 50%   | Avatars, FAB       |
