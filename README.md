# Mato Here — PWA Arcade Game

A lightweight English-language arcade game: click/tap falling crates to discover gifts and avoid bombs.

## Features
- 60-second rounds, three lives, gifts (+10), empty crates (+2), bombs (-1 life)
- Increasing difficulty, high scores saved locally, pause, sound toggle
- Responsive canvas, mouse/touch support, offline caching after first load
- No external libraries, trackers, advertisements, or network APIs

## Publish on GitHub Pages
1. Create a public GitHub repository called `mato-here`.
2. Upload **the contents of this folder** to the repository root (including `icons`).
3. In Settings > Pages, select Deploy from a branch, `main`, `/(root)`.
4. Open `https://YOUR-USERNAME.github.io/mato-here/` and verify play and install.

## Package for Microsoft Store
1. Paste your deployed HTTPS URL into https://www.pwabuilder.com/.
2. Check PWA manifest/service worker and select Windows packaging.
3. Download the generated Windows package, test it, and submit via Microsoft Partner Center.
4. If `runFullTrust` is present, Microsoft may require a restricted-capability justification. Provide an accurate explanation or remove it only if the package can function without it.
5. Upload real gameplay screenshots, a privacy policy reflecting actual behavior, and accurate product information.

## Privacy notes
The game does not collect personal data, send scores to servers, or use third-party services. Best score is stored in localStorage on the device. Hosting providers may independently log website requests.

## Files
- `index.html`: app shell
- `style.css`: UI styles
- `game.js`: gameplay
- `manifest.webmanifest`: install metadata
- `sw.js`: offline cache
- `icons/`: PWA icons
