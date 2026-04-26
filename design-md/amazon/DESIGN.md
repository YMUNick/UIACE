# Design System Inspiration of Amazon

## 1. Visual Theme & Atmosphere

Amazon's design is a high-density, commerce-first system built around conversion. The interface uses a white (#FFFFFF) canvas with a distinctive two-layer header: a deep navy (#232F3E) primary bar and a secondary navy bar (#37475A) for navigation categories. The primary brand color — Amazon Orange (#FF9900) — is reserved exclusively for CTAs like "Add to Cart" and "Buy Now", creating immediate visual hierarchy toward purchase actions.

Typography uses Amazon Ember — a proprietary humanist sans-serif designed for legibility across the vast variety of product pages, descriptions, and dense listing grids. In the absence of Amazon Ember, Arial and system fonts provide a dense, functional fallback. Font weights are straightforward: 400 for product titles and body, 700 for headings and buttons.

Border radius is minimal (3–4px) compared to modern design systems, reflecting Amazon's utility-first philosophy where clarity and density outweigh aesthetic softness. The orange focus ring and inset shadows on form inputs are distinctly Amazonian.

**Key Characteristics:**
- Orange (#FF9900) exclusively for primary CTAs — maximum purchase intent clarity
- Two-tone navy header: primary (#232F3E) + category bar (#37475A)
- Teal link color (#007185) for product titles and navigation — distinct from orange CTAs
- Minimal border radius: 3px buttons, 4px cards — utilitarian not decorative
- Dense information layout: ratings, price, delivery info all in card footers
- Inset box-shadow on form inputs for a tactile, pressed feel
- Star rating as primary social proof signal

## 2. Color Palette & Roles

### Brand
- **Amazon Orange** (`#FF9900`): Primary CTA — Add to Cart, Buy Now
- **Orange Dark** (`#E47911`): Pressed/hover state for orange CTAs
- **Amazon Navy** (`#232F3E`): Primary header background
- **Navy Mid** (`#37475A`): Category navigation bar, hover states

### Text & Interactive
- **Near Black** (`#0F1111`): Primary text — slightly cool, not pure black
- **Secondary** (`#565959`): Supporting text, product metadata
- **Teal Link** (`#007185`): Product titles, navigation links, "See all" CTAs

### Surface
- **Surface** (`#F7F8F8`): Page background
- **Surface 2** (`#EAEDED`): Secondary backgrounds, table rows
- **Border** (`#D5D9D9`): Card borders, input borders, dividers

### States
- **Error** (`#CC0C39`): Error messages, out-of-stock states

### Dark Mode
- Background: `#0F1111`, Surface: `#1A1A1A`
- Text: `#CCCCCC`, Secondary: `#8F9191`
- Link shifts to `#00A8CC`, Error to `#FF6B6B`

## 3. Typography

**Typeface:** Amazon Ember → Arial (fallback)

| Role         | Size | Weight | Notes                     |
|--------------|------|--------|---------------------------|
| Heading      | 26px | 700    | Section, page titles      |
| Title        | 20px | 700    | Widget, carousel headers  |
| Product Name | 16px | 400    | Teal link color            |
| Body         | 14px | 400    | Descriptions, body copy   |
| Label        | 12px | 400    | Shipping, metadata        |
| Caption      | 11px | 400    | Fine print, disclaimers   |

## 4. Components

### Buttons
- **Primary** (Orange): `#FF9900` bg, `#0F1111` text, 3px radius, `#C45500` border — all purchase actions
- **Secondary**: `#EAEDED` bg, neutral text, 3px radius — secondary actions
- **Link**: no bg/border, `#007185` teal — inline navigation

### Cards (Product)
- Border: `1px solid #D5D9D9`
- Shadow: `0 2px 5px 0 rgba(213,217,217,0.5)` — soft, warm
- Border radius: 4px
- Content: product image → title (link) → price → ratings/delivery

### Forms
- 3px radius, `1px #D5D9D9` border
- Inset shadow: `0 1px 2px rgba(15,17,17,0.15) inset`
- Focus: `#FF9900` border + `rgba(255,153,0,0.25)` 3px ring

## 5. Spacing & Layout

8px base grid. Common values: 4, 8, 12, 16, 24, 32px. Dense column-based product grids with minimal whitespace.

## 6. Border Radius

| Value | Usage        |
|-------|--------------|
| 3px   | Buttons      |
| 4px   | Cards, tags  |
| 8px   | Badges       |
| 50%   | Avatar       |
