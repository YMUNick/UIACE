# Design System Inspiration of Netflix

## 1. Visual Theme & Atmosphere

Netflix's design is a cinematic, dark-first system built around content supremacy. The interface uses deep near-black (#141414) as the primary canvas — dark enough to recede and let thumbnails and video content pop. The singular brand accent is Netflix Red (#E50914), appearing in the logo, Play button, and focus states. Everything else is neutral — grays, blacks, and white text.

The design is intentionally minimal outside of content areas. Buttons are sharply rectangular (4px radius), typography is heavy (800 weight for titles), and content cards are tight and grid-aligned for efficient browsing density. The iconic two-button pattern — red "Play" + gray "More Info" — appears throughout as the primary CTA combination.

**Key Characteristics:**
- Netflix Red (#E50914) as the single brand accent on near-black (#141414) canvas
- Two-button CTA pattern: Play (red) + More Info (gray semi-transparent)
- Heavy typography (Inter 800) — cinematic, authoritative
- Flat 4px radius — sharp, modern, content-forward
- Dark mode is the canonical experience; light mode is secondary
- Card hover scale effect for content browsing feedback
- Progress bar (2px height, red) for watched content

## 2. Color Palette & Roles

### Brand
- **Netflix Red** (`#E50914`): Logo, Play button, focus ring
- **Red Dark** (`#B20710`): Pressed/hover state
- **Netflix Black** (`#141414`): Primary background
- **More Info Gray** (`rgba(109,109,110,0.7)`): Secondary button

### Surface & Text
- **On Background** (`#FFFFFF`): Primary text on dark
- **Secondary** (`#AAAAAA`): Metadata, labels
- **Surface** (`#1F1F1F`): Card and panel background
- **Surface 2** (`#2A2A2A`): Elevated surfaces
- **Border** (`#333333`): Dividers

### Light Mode
- Background: `#FFFFFF`, Surface: `#F3F3F3`
- Text: `#141414`, Secondary: `#555555`

## 3. Typography

**Typeface:** Inter (Netflix uses Netflix Sans — custom, not public)

| Role    | Size | Weight | Notes            |
|---------|------|--------|------------------|
| Display | 30px | 800    | -0.5px tracking  |
| Title   | 22px | 800    | -0.3px tracking  |
| Section | 16px | 700    | Row headers      |
| Body    | 14px | 400    | Descriptions     |
| Label   | 12px | 500    | Episode metadata |
| Caption | 11px | 400    | Technical info   |

## 4. Components

### Buttons
- **Play (Primary)**: Red bg, white text, 4px radius, play icon
- **More Info (Secondary)**: `rgba(109,109,110,0.7)` bg, white text, 4px radius
- **Outlined**: transparent, white border/text, 4px radius
- **FAB**: circular red, play icon

### Cards (Content)
- Border radius: 4px — sharp, content-forward
- Hover: `scale(1.03)` + heavier shadow — browse affordance
- Tight grid: 16/9 aspect ratio thumbnails

### Forms
- Surface-colored bg, 2px border
- Focus: dark/white border (not red — avoids confusion with error)
- Error: red border

## 5. Spacing & Layout

8px base grid. Tight card grids (8px gap) for content density. Generous section padding (48px+).

## 6. Border Radius

| Value | Usage             |
|-------|-------------------|
| 2px   | Progress bar      |
| 4px   | Buttons, cards    |
| 8px   | Modals, dialogs   |
| 50%   | Avatar profiles   |
