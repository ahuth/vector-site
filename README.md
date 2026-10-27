# Vector site

A static landing page for the Vector desktop app. Everything lives in `index.html`: markup, styles, and inline SVG. No build step, JavaScript, dependencies, external fonts, or tracking.

## Preview

Open `index.html` in a browser, or run `python3 -m http.server 8000` from this directory and visit http://localhost:8000.

## Publish

Serve this directory with any static host. Only `index.html` is needed.

Download buttons point to `https://github.com/ahuth/vector-issues/releases/latest`, matching the app’s configured public release repository. Feedback links point to that repository’s issues. Confirm a public release with a downloadable macOS installer is available before launch; live availability could not be verified during implementation. The page lists macOS 13+ and Apple silicon based on the app configuration and release workflow.

The workspace preview is an HTML/CSS illustration, not an app screenshot. Edit copy, colors, and links directly in `index.html`.
