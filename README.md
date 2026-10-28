# Vector site

A static landing page for the Vector beta. Everything lives in `index.html`: markup, styles, inline SVG, and a small inline script (starfields and the email form). No build step, dependencies, or web fonts. Type and colors match the Vector app: the system UI font and the palette from the app's `frontend/src/styles.css`.

`sketch.html` is an alternate "hand-drawn engineering diagram" direction, kept for reference. Delete it once you're settled.

`directions.html` contains three simpler graphite alternatives. Use the top navigation to compare Statement (typography and a blue orbital accent), Architecture (an amber system diagram), and Workbench (a focused illustrative conversation). Each direction has a linkable URL fragment, uses 16px minimum text, and supports reduced motion. The existing landing page is unchanged.

`explorations.html` adds four further concepts: Bearing (a directional instrument), Redline (an editorial correction), Field (an interactive field of arrows), and Section (an exploded architectural drawing). Both concept pages link to each other. Field’s “Set direction” button aligns the arrows; the other illustrations use restrained motion with reduced-motion support.

`options/` holds four full-page alternatives that are simpler and punchier: Blueprint, Spotlight, Undercurrent, and Titanium. They share `options/shared.css`. Text is 16px or larger. A switcher at the bottom of each page moves between them, and should be removed when one is promoted to `index.html`.

## Preview

Open `index.html` in a browser.

## Publish

Serve this directory with any static host. `index.html` and the `assets/` folder (app icon, favicon) are all that's needed.

- Download buttons point to `https://github.com/ahuth/vector-issues/releases/latest`. Feedback links point to that repository's issues.
- The "Notify me" email form posts to `SIGNUP_ENDPOINT` near the bottom of `index.html`. It's empty by default. Until you set it, submitting shows a "not connected yet" message. Any form backend that accepts a `POST` with an `email` field works (Formspree, Buttondown, Loops, etc.).
- The app window in the hero is an HTML/CSS illustration, not a screenshot.

The icons in `assets/` are resized from `src-tauri/icons/icon.png` in the Vector repo.
