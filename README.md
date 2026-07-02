# Minimalist Weather Widget

A beautiful, scalable, and ultra-minimalist weather widget inspired by Notion's aesthetics. Built entirely with vanilla HTML, CSS, and JavaScript in a single portable file, making it extremely easy to embed in custom dashboards, Notion pages, or iframe-compatible workspaces.

## Features

- **Notion-Inspired Aesthetic:** Clean monochrome color schemes, subtle hover transitions, and Inter typography designed to blend perfectly with modern digital workspaces.
- **Dynamic Container Query Sizing:** Uses modern CSS Container Queries to scale and adjust layouts dynamically based on parent container size:
  - **Wide Landscape:** Spaced out row format, ideal for headers or horizontal sections.
  - **Medium Square:** Compact block format, ideal for sidebar components.
  - **Narrow Portrait:** Vertical stacked format, ideal for mobile or narrow side margins.
- **Automatic Geolocation Detection:** Automatically detects the user's location on startup using the browser's Geolocation API, with robust fallback chains to IP-based geolocation.
- **Interactive City Search:** Click the city name to type and search for any location worldwide. Selected locations are saved in `localStorage` for future visits.
- **Embedded vs. Standalone Modes:** Automatically detects if loaded inside an iframe and configures appropriate margins, borders, and rounded corners.
- **Fullscreen API support:** A subtle fullscreen expand/collapse toggle in the bottom right corner.
- **Adaptive Dark Mode:** Dynamically listens to browser themes (`prefers-color-scheme: dark`) to adjust backgrounds, borders, and monochrome SVGs.

## Files

- [index.html](index.html): The complete single-file widget code.
- [test_iframe.html](test_iframe.html): Responsive testing harness displaying the widget in wide, medium, and narrow layout formats inside iframes.

## Setup & Deployment

1. **Local Run:** Open [index.html](index.html) directly in any modern web browser.
2. **Iframe Testing:** Open [test_iframe.html](test_iframe.html) to preview the widget rendering in all three responsive layout modes.
3. **Embed in Notion:** Deploy the `index.html` to any static hosting provider (e.g. GitHub Pages, Vercel, Netlify) and embed the URL directly inside Notion.
