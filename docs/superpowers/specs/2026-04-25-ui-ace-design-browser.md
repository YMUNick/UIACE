# UI Ace — Design Style Browser

**Date:** 2026-04-25
**Status:** Approved

## Overview

A single-file static web app (`index.html`) that lets users browse 58 company design styles. The homepage is styled with Airbnb's design system. Clicking a company slides in a preview panel showing that company's existing `preview.html` or `preview-dark.html` file in an iframe. No build tools, no npm, no dependencies — pure HTML/CSS/JS.

## Architecture

```
UI_Ace/
  index.html          ← the entire app
  design-md/
    airbnb/
      preview.html
      preview-dark.html
    apple/
      preview.html
      preview-dark.html
    ... (58 companies total)
```

`index.html` links to files in `design-md/` via relative paths. The `design-md/` directory is not modified.

## Homepage

### Style
Airbnb design system:
- Font: `Nunito Sans` from Google Fonts (weights 400, 500, 600, 700)
- Colors: white background `#ffffff`, near-black text `#222222`, brand accent `#ff385c` (Rausch Red)
- Card shadows: `rgba(0,0,0,0.02) 0px 0px 0px 1px, rgba(0,0,0,0.04) 0px 2px 6px, rgba(0,0,0,0.1) 0px 4px 8px`
- Border radius: 14px on cards

### Header
Sticky top bar, white background, `1px solid #ebebeb` bottom border.
- Left: "UI Ace" logotype in Rausch Red
- Right: nothing (clean, Airbnb-style)

### Hero
Centered, 48px top padding:
- Headline: "Browse Design Styles" (28px, 700 weight)
- Subtitle: "58 company design systems — light & dark" (16px, secondary gray)
- Search input: full-width max 480px, rounded pill, 1px border, filters company cards in real-time

### Company Grid
`display: grid; grid-template-columns: repeat(auto-fill, minmax(160px, 1fr)); gap: 16px`

Each card:
- White background, Airbnb card shadow, 14px border radius
- Favicon: `<img src="https://www.google.com/s2/favicons?domain=<domain>&sz=64">` — 40px square, centered
- Company name: 13px, 600 weight, near-black, centered
- Hover: shadow lifts (`rgba(0,0,0,0.08) 0px 4px 12px`), slight translateY(-2px), cursor pointer
- `data-company` attribute for search filtering

### Domain Mapping
Folder name → favicon domain (overrides where folder name ≠ domain):

| Folder | Domain |
|--------|--------|
| airbnb | airbnb.com |
| airtable | airtable.com |
| apple | apple.com |
| bmw | bmw.com |
| cal | cal.com |
| claude | claude.ai |
| clay | clay.run |
| clickhouse | clickhouse.com |
| cohere | cohere.com |
| coinbase | coinbase.com |
| composio | composio.io |
| cursor | cursor.com |
| elevenlabs | elevenlabs.io |
| expo | expo.dev |
| ferrari | ferrari.com |
| figma | figma.com |
| framer | framer.com |
| hashicorp | hashicorp.com |
| ibm | ibm.com |
| intercom | intercom.com |
| kraken | kraken.com |
| lamborghini | lamborghini.com |
| linear.app | linear.app |
| lovable | lovable.dev |
| minimax | minimaxi.com |
| mintlify | mintlify.com |
| miro | miro.com |
| mistral.ai | mistral.ai |
| mongodb | mongodb.com |
| notion | notion.so |
| nvidia | nvidia.com |
| ollama | ollama.com |
| opencode.ai | opencode.ai |
| pinterest | pinterest.com |
| posthog | posthog.com |
| raycast | raycast.com |
| renault | renault.com |
| replicate | replicate.com |
| resend | resend.com |
| revolut | revolut.com |
| runwayml | runwayml.com |
| sanity | sanity.io |
| sentry | sentry.io |
| spacex | spacex.com |
| spotify | spotify.com |
| stripe | stripe.com |
| supabase | supabase.com |
| superhuman | superhuman.com |
| tesla | tesla.com |
| together.ai | together.ai |
| uber | uber.com |
| vercel | vercel.com |
| voltagent | voltagent.dev |
| warp | warp.dev |
| webflow | webflow.com |
| wise | wise.com |
| x.ai | x.ai |
| zapier | zapier.com |

## Slide-in Preview Panel

### Behavior
- Clicking a card sets `panel.style.transform = 'translateX(0)'` (slides in from right)
- Panel width: 85vw, positioned `fixed` right-0, top-0, height 100vh
- Transition: `transform 300ms ease`
- A semi-transparent backdrop covers the remaining 15% left; clicking it closes the panel
- Panel is always in the DOM; default state is `translateX(100%)`

### Panel Top Bar
Sticky, white, `1px solid #ebebeb` bottom border, Airbnb-styled:
- Left: company favicon (20px) + company name (14px, 600 weight)
- Center: Light/Dark toggle pill — two buttons inside a rounded container; active state uses `#ff385c` background
- Right: `✕` close button (circular, 36px)

### iframe
- `width: 100%; height: calc(100vh - 48px); border: none`
- `src` switches between `design-md/<company>/preview.html` (light) and `design-md/<company>/preview-dark.html` (dark) based on toggle state

### Default toggle state: Light

## Search
- Input event listener on the search field
- Filters company cards by `textContent` match (case-insensitive)
- Non-matching cards get `display: none`
- Clears automatically when the panel closes

## JavaScript
- No frameworks, no modules — single inline `<script>` at bottom of `<body>`
- State: `currentCompany` (string), `currentMode` ('light' | 'dark')
- Functions: `openCompany(folder, name, domain)`, `closePanel()`, `setMode(mode)`, `filterCards(query)`

## Files to create
- `index.html` — the entire application
- `.gitignore` entry for `.superpowers/`
