# Vector site

A static landing page for the Vector beta. Everything lives in `index.html`: markup, styles, inline SVG, and a small inline script (starfields and the email form). No build step, dependencies, or web fonts. Type and colors match the Vector app: the system UI font and the palette from the app's `frontend/src/styles.css`.

`sketch.html` is an alternate "hand-drawn engineering diagram" direction, kept for reference. Delete it once you're settled.

## Preview

Open `index.html` in a browser.

## Publish

Serve this directory with any static host. `index.html` and the `assets/` folder (app icon, favicon) are all that's needed.

- Download buttons point to `https://github.com/ahuth/vector-issues/releases/latest`. Feedback links point to that repository's issues.
- The "Notify me" email form posts to `SIGNUP_ENDPOINT` near the bottom of `index.html`. It's empty by default. Until you set it, submitting shows a "not connected yet" message. Any form backend that accepts a `POST` with an `email` field works (Formspree, Buttondown, Loops, etc.).
- The app window in the hero is an HTML/CSS illustration, not a screenshot.

The icons in `assets/` are resized from `src-tauri/icons/icon.png` in the Vector repo.
