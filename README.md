# Pocket Ledger

A monthly budget that follows the 50/30/20 rule, in Thunder Plus’s IDM skin (warm grey paper, ink frames, Inter + JetBrains Mono, bundled in `fonts/`).

- Enter your monthly take-home pay once; it splits into three envelopes: **Needs** (50%), **Wants** (30%) and **Savings & debt** (20%). Other splits (60/20/20, 70/20/10, 40/30/30) are in Settings.
- Log a purchase with an amount and a word or two. The category picks itself from the description (rent, groceries → Need; 401k, savings → Save); anything else stays on the last category you tapped (Need to start).
- **Saved costs**: like the Daily meds pickers, keep a list of costs you log often (name, usual amount, category). Pick one from **Pick a saved cost…** to fill in the form, or choose **+ New saved cost…** to save what you've typed. Edit or delete them in the Saved costs box.
- **Repeat**: Once, Daily, Weekly or Monthly. A repeat starts on the chosen date (monthly ones on the 31st land on the last day of shorter months). Tap × on one to skip just that one; tap the row to skip, stop after it, bring skipped ones back, change it, or delete them all.
- **Extra income**: log one-off money (a gig, a sale, a refund) by month. It's added to that month's pay before the envelopes are split.
- **Three logs**, each grouped by day with its own total at the top: **Needs** (grey, in its own column), **Purchases** (wants) and **Savings** (green). A **Grand total** box above them adds all three. Tap any cost to edit its amount, name, category or date (with undo); × deletes it.
- **Month-end rollover**: when a month is over, any pay or extra income that wasn't spent or saved goes into that month's savings automatically ("Unspent from October"). It starts from the first month you logged anything.
- **Past savings** and **Deduct from savings**: at the bottom of the Savings log, add money saved before Pocket Ledger (or outside it), or take money out of savings. **Saved to date** adds past savings, every savings entry and every rollover up to today, minus anything taken out. Neither changes a month's envelopes.
- Each month has delete and undo. Swipe left or right (as in Daily meds) or use the arrows to change month; when you flip to another month, the date fields follow, so you can plan ahead without being bounced back to this month.
- Works offline and installs as an app (the **Install app** button at the top, or Share → Add to Home Screen on iPhone).

Everything is stored on the device in `localStorage`. Use **Copy backup** / **Restore pasted backup** in Settings to move data between devices or browsers.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: markup, styles and script |
| `manifest.webmanifest` | App name, icons and colors for installing |
| `sw.js` | Service worker: offline cache and update check. Bump `CACHE` whenever `index.html` changes |
| `icon.svg`, `icon-*.png` | App icon in the IDM skin: an ink-framed panel on grey paper, its title strip carrying the orange dot and the needs / wants / savings marks, with the split-coin dollar sign in ink |

## Hosting

GitHub Pages from the `main` branch, root folder: Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`.
