# Alchemist Labs

AI Brand Studio. Every constraint is a door, not a wall.

**Live site:** [alchemist-studio.github.io](https://alchemist-studio.github.io/)

A responsive landing page built with plain HTML, CSS, JavaScript, and SVG.
No package installation or build step is required.

## Features

- Three color palettes: Oxide, Indigo, and Carbon.
- Theme-aware favicon and browser theme color.
- Responsive desktop and mobile layouts.
- Keyboard-accessible theme controls and visible focus indicators.
- Styles for reduced-motion and increased-contrast preferences.
- Locally hosted DM Sans fonts.

## Preview locally

For a quick preview, open `index.html` in your browser.

Alternatively, if Python 3 is installed, run a local web server from the
repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open [localhost:8000](http://localhost:8000).
Press `Ctrl+C` in the terminal to stop the server.

## Project structure

```text
index.html               Page content, theme controls, and inline SVG logo
alchemist-labs.css       Layout, typography, responsive styles, and palettes
alchemist-labs.js        Theme switching, browser theme color, and favicon updates
alchemist-labs-icon.svg  Default favicon
fonts/                   Bundled DM Sans fonts and license
.nojekyll                Disables Jekyll processing for GitHub Pages
```

## Making changes

### Content and navigation

Edit `index.html` to update the headline, studio name, navigation links,
page title, or description.

The main logo is an inline SVG in this file. The default favicon is stored
separately in `alchemist-labs-icon.svg`.

### Layout and typography

Edit `alchemist-labs.css` to adjust spacing, type sizes, and responsive
layouts. Font declarations appear at the top of the stylesheet.

### Color themes

The default Oxide palette is defined in `:root` in `alchemist-labs.css`.
Indigo and Carbon override those variables using `html[data-theme="…"]`
selectors.

`alchemist-labs.js` applies the selected theme and updates the browser theme
color and favicon. Keep its color values and theme-specific icons consistent
with the CSS palettes.

When adding a theme, also add a corresponding radio control in `index.html`.

Theme choices are not currently saved explicitly between visits.

## Before publishing

There is no automated test suite included. After making a change:

- Check both desktop and narrow mobile layouts for overflow or clipped text.
- Try all three themes and confirm the selected control and page colors agree.
- Check that the favicon updates with the selected theme.
- Use the keyboard to reach the theme picker and navigation links; use the
  arrow keys to change the selected theme.
- Confirm focus indicators remain visible.
- Check the page with reduced motion enabled.
- Confirm the Showcase and Approach links point to the intended destinations.
- Confirm the page content remains readable with JavaScript disabled.

## Publishing

This repository serves the site through GitHub Pages.

Changes pushed to `main` publish from the repository root. No build command
or generated output directory is required.

After deployment, check the live site to confirm the changes appear as
expected.

## Fonts and licensing

DM Sans is bundled locally under the SIL Open Font License.
See [the font license](fonts/DM-Sans-LICENSE.txt) for details.

That license applies to the bundled fonts; it does not establish a license
for the rest of this repository.
