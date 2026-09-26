# Alchemist Labs

AI Brand Studio. Every constraint is a door, not a wall.

The Alchemist Labs landing page, built with plain HTML, CSS, JavaScript,
and SVG. No framework, package installation, or build step is required.

[Visit the website](https://alchemist-studio.github.io/) ·
[Showcase](https://dribbble.com/alchemist-studio) ·
[Approach](https://eoncodes.substack.com/p/the-three-steps-behind-every-original)

## Features

- Three color palettes: Oxide, Indigo, and Carbon.
- Theme switching that updates the page, favicon, and browser theme color.
- Responsive layouts for desktop and mobile.
- SVG brand artwork with geometric construction details.
- Locally hosted DM Sans fonts.
- Keyboard-operable theme controls and visible focus indicators.
- Styles that respect reduced-motion and increased-contrast preferences.

## Preview locally

Clone the repository:

```sh
git clone https://github.com/alchemist-studio/alchemist-studio.github.io.git
cd alchemist-studio.github.io
```

Open `index.html` directly in your browser, or serve the repository locally.
For example, with Python 3 installed:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Visit [http://127.0.0.1:8000](http://127.0.0.1:8000).
Stop the server with `Ctrl+C`.

## Project structure

```text
.
├── index.html                 # Page content, metadata, and inline SVG artwork
├── alchemist-labs.css         # Typography, palettes, and responsive styles
├── alchemist-labs.js          # Theme switching and dynamic favicon updates
├── alchemist-labs-icon.svg    # Default favicon
├── fonts/
│   ├── dm-sans-400.ttf        # Regular font weight
│   ├── dm-sans-500.ttf        # Medium font weight
│   └── DM-Sans-LICENSE.txt    # Font license
├── .nojekyll
└── README.md
```

## Making changes

- **Content and links:** Edit `index.html`.
- **Layout and typography:** Edit `alchemist-labs.css`.
- **Theme colors:** Update the CSS palette variables and the corresponding
  theme-color and favicon definitions in `alchemist-labs.js`.
- **Brand artwork:** The main symbol is inline in `index.html`. Favicon
  artwork also appears in `alchemist-labs-icon.svg` and the theme-specific
  data URLs in `alchemist-labs.js`.
- **Search metadata:** Update the title, description, and canonical URL
  in the `<head>` of `index.html` as needed.

Refresh the browser after saving changes. There is no compilation step.

## Before publishing

The repository does not currently include an automated test suite.
Use this manual checklist when reviewing changes:

- [ ] Check desktop and mobile layouts for clipping or horizontal overflow.
- [ ] Switch between Oxide, Indigo, and Carbon.
- [ ] Confirm the favicon changes with the selected theme.
- [ ] Navigate links and theme controls using the keyboard.
- [ ] Check reduced-motion and increased-contrast behavior.
- [ ] Confirm the Showcase and Approach links point to the intended pages.
- [ ] Check the browser console and network panel for errors or missing assets.

## Publishing

The site is served through GitHub Pages from the repository root on `main`.

Changes pushed or merged into `main` are published without a local build
step. After deployment finishes, check the live website to confirm the
updated content and assets appear correctly.

## Typography

DM Sans is bundled locally in regular (`400`) and medium (`500`) weights
under the SIL Open Font License.

See [the font license](fonts/DM-Sans-LICENSE.txt) for details.
