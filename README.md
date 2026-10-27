# Pocket Ledger

A monthly budget that follows the 50/30/20 rule, styled like Daily meds.

- Enter your monthly take-home pay once; it splits into three envelopes: **Needs** (50%), **Wants** (30%) and **Savings & debt** (20%). Other splits (60/20/20, 70/20/10, 40/30/30) are in Settings.
- Log a purchase with an amount and a word or two. The category picks itself from the description (rent, groceries → Need; 401k, savings → Save); anything else stays on the last category you tapped (Need to start).
- **Saved costs**: like the Daily meds pickers, keep a list of costs you log often (name, usual amount, category). Pick one from **Pick a saved cost…** to fill in the form, or choose **+ New saved cost…** to save what you've typed. Edit or delete them in the Saved costs box.
- **Repeat**: Once, Daily, Weekly or Monthly. A repeat starts on the chosen date (monthly ones on the 31st land on the last day of shorter months). Tap × on one to skip just that one; tap the row to skip, stop after it, bring skipped ones back, change it, or delete them all.
- **Extra income**: log one-off money (a gig, a sale, a refund) by month. It's added to that month's pay before the envelopes are split.
- Purchases are listed by day for each month, with delete and undo. Swipe left or right (as in Daily meds) or use the arrows to change month; when you flip to another month, the date fields follow, so you can plan ahead without being bounced back to this month.
- Works offline and installs as an app (the **Install app** button at the top, or Share → Add to Home Screen on iPhone).

Everything is stored on the device in `localStorage`. Use **Copy backup** / **Restore pasted backup** in Settings to move data between devices or browsers.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: markup, styles and script |
| `manifest.webmanifest` | App name, icons and colors for installing |
| `sw.js` | Service worker: offline cache and update check. Bump `CACHE` whenever `index.html` changes |
| `icon.svg`, `icon-*.png` | App icon: an abstract dollar sign (a pink coin split and slipped along a bar) with fading teal and lavender shadows |

## Hosting

GitHub Pages from the `main` branch, root folder: Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`.
