# Ambika Real Estate — Promotional Email

A responsive HTML email promoting a premium 3400 sq ft commercial rental space in Chakan MIDC. Built with [MJML](https://mjml.io) for desktop & mobile-friendly layouts.

## Project Structure

```
├── src/
│   └── emails/
│       └── promotional-offer.mjml   # Email source (MJML)
├── dist/
│   └── promotional-offer.html        # Compiled output (inline-styled HTML)
├── package.json
├── .gitignore
└── README.md
```

## Setup

```bash
npm install
```

## Build

```bash
npm run build
```

Compiles `src/emails/promotional-offer.mjml` → `dist/promotional-offer.html`.

## Sending the Email

1. Open `dist/promotional-offer.html` in a text editor and copy the full contents
2. Paste into [Putsmail](https://putsmail.com) (HTML tab) and send a test to your inbox
3. Or use Gmail's "Edit as HTML" dev tools method (see below)

### Gmail Workaround

Gmail strips document shell tags on paste. Use the content inside `<body>` only:
- Open `dist/promotional-offer.html` and remove the `<html>`, `<head>`, `<body>` wrappers
- Paste the remaining `<div>` block into Gmail's "Edit as HTML" (right-click compose area → Inspect → right-click the editable `<div>` → Edit as HTML → paste)

**Recommended:** Use Putsmail — it handles this automatically.

## Customization

Edit `src/emails/promotional-offer.mjml` and rebuild:

| Token | Color | Hex |
|---|---|---|
| Brand primary | Orange | `#FFA500` |
| Brand dark | Deep orange | `#ED8A00` |
| Text (Real Estate) | Sky blue | `#4cbdff` |
| Text (dark) | Charcoal | `#1F2937` |
| Text (muted) | Gray | `#6B7280` |
| Background | Light gray | `#F3F4F6` |

## Brand Assets

- **Logo:** `https://ambika-real-estate.vercel.app/_app/immutable/assets/ambika_logo.DEwhPv4J.png`
- **Building Photo:** `https://ambika-real-estate.vercel.app/_app/immutable/assets/Premium%20Building%20Photo.1UXdpFPh.jpeg`
- **Website:** `https://ambika-real-estate.vercel.app/`
- **YouTube Short:** `https://www.youtube.com/shorts/WPxrUGJySt8`

## Tech Stack

- [MJML](https://mjml.io) v4 — responsive email framework
- Node.js — build tooling
