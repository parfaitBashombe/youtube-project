# YouTube Clone

A front-end clone of the YouTube homepage built with pure HTML and vanilla CSS — no JavaScript, no frameworks, no dependencies.

The goal of this project is to practice core CSS layout techniques including Flexbox, CSS Grid, fixed positioning, responsive design, and hover effects by faithfully replicating the YouTube UI.

---

## Project Structure

```
youtube-project/
├── index.html
├── styles/
│   ├── general.css       # CSS variables (design tokens), box-sizing reset, base body
│   ├── typography.css    # Global font rules, video title clamp, author and stats text
│   ├── header.css        # Fixed top navigation bar
│   ├── sidebar.css       # Fixed left sidebar panel
│   └── preview.css       # Video grid layout and individual video card styles
├── icons/                # SVG icons and user avatar
├── thumbails/            # Video thumbnail images (.webp)
└── channel-pictures/     # Channel profile photos
```

---

## Features

- Fixed header with pill-shaped search bar, voice search, icon buttons with tooltips, and a notification badge
- Fixed compact sidebar with icon and label navigation links, hover highlight
- Responsive video grid that adapts from 1 to 4 columns depending on viewport width
- Video cards with rounded thumbnails, circular channel avatars, 2-line title clamp, and a video duration badge
- CSS custom properties (design tokens) for consistent colors, spacing, and sizing across all stylesheets
- Light theme only, using the Roboto typeface via Google Fonts

---

## CSS Architecture

Each stylesheet has a single, focused responsibility:

| File | Responsibility |
|---|---|
| `general.css` | Design tokens, reset, body |
| `typography.css` | All font and text styles |
| `header.css` | Header component |
| `sidebar.css` | Sidebar component |
| `preview.css` | Video card and grid |

Stylesheets are loaded in dependency order: `general` then `typography` then components.

---

## Responsive Breakpoints

| Viewport width | Grid columns |
|---|---|
| Up to 600px | 1 column |
| 601px – 900px | 2 columns |
| 901px – 1200px | 3 columns |
| 1201px and above | 4 columns |

---

## Getting Started

No build step required. Open `index.html` directly in any modern browser.

```bash
open index.html
```

---

## Technologies

- HTML5
- CSS3 (Flexbox, CSS Grid, custom properties, media queries)
- Google Fonts — Roboto
