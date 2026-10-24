# Pocket Ledger

A monthly budget that follows the 50/30/20 rule, styled like Daily meds.

- Enter your monthly take-home pay once; it splits into three envelopes: **Needs** (50%), **Wants** (30%) and **Savings & debt** (20%). Other splits (60/20/20, 70/20/10, 40/30/30) are in Settings.
- Log a purchase with an amount and a word or two. The category picks itself from the description (rent, groceries → Need; 401k, savings → Save; everything else → Want) and can be changed with one tap.
- Purchases are listed by day for each month, with delete and undo.
- Works offline and installs as an app (the **Install app** button at the top, or Share → Add to Home Screen on iPhone).

Everything is stored on the device in `localStorage`. Use **Copy backup** / **Restore pasted backup** in Settings to move data between devices or browsers.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: markup, styles and script |
| `manifest.webmanifest` | App name, icons and colors for installing |
| `sw.js` | Service worker: offline cache and update check. Bump `CACHE` whenever `index.html` changes |
| `icon.svg`, `icon-*.png` | App icon: the three category shapes (square = needs, circle = wants, diamond = savings) |

## Hosting

GitHub Pages from the `main` branch, root folder: Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`.
