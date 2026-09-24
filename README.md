# Alchemist Labs

The landing page for Alchemist Labs, an AI brand studio.

> Every constraint is a door, not a wall.

Visit the [live site](https://alchemist-studio.github.io/).

## About the site

This is a single-page, static site built with HTML, CSS, JavaScript, and SVG.
It has no dependencies or build step. The page features an illustrated studio
symbol, links to the studio's showcase and approach, and three selectable color
palettes: Oxide, Indigo, and Carbon. The layout adapts to desktop and mobile
screens, with support for reduced-motion and increased-contrast preferences.

## Files

| Path | Purpose |
| --- | --- |
| `index.html` | Page content, navigation, and inline symbol artwork |
| `alchemist-labs.css` | Layout, typography, color palettes, and responsive styles |
| `alchemist-labs.js` | Palette switching, browser theme color, and matching favicon |
| `alchemist-labs-icon.svg` | Default favicon |
| `fonts/` | Locally hosted DM Sans fonts and their license |
| `.nojekyll` | Serves the files directly on GitHub Pages |

## Preview locally

From the repository root, start a static file server:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/` in a browser. Stop the server with Ctrl+C.
No package installation is needed.

## Publishing

GitHub Pages publishes the repository root from `main`. Changes pushed to that
branch are served at the live site; there is no build or deployment command.

DM Sans is bundled locally under the SIL Open Font License. See the
[font license](fonts/DM-Sans-LICENSE.txt).
