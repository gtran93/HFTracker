# TradeCommand 360 — Debugged Build

This is a rebuilt offline-first trade tracking app for Live and Demo binary-options journalling.

## Files
- `index.html` — main app, fully self-contained UI/CSS/JS.
- `manifest.json` — PWA metadata.
- `sw.js` — offline cache service worker when served from HTTP/HTTPS.
- `icon-192.png`, `icon-512.png` — app icons.

## What was fixed and rebuilt
- Fixed the Live/Demo page crash caused by undefined roadmap variables.
- Rebuilt the balance engine so Live and Demo balances are separated and recalculated safely.
- Added balance-sync entries instead of silent balance overrides.
- Removed dependency on external Chart.js so the dashboard works offline.
- Added SVG equity and daily P/L charts.
- Added Live/Demo trade logger, dashboard, roadmap, financial goals, discipline guard, data export/import, CSV export, and PWA support.
- Added user-friendly animations, glowing theme, progress bars, cards, toasts, modals, and mobile-first layout.

## How to use
Open `index.html` in a browser. For best PWA/offline behaviour, serve the folder through a local or hosted HTTP server, then add it to your phone home screen.

## Data note
All trade data is stored locally in the browser. Use **Settings → Export JSON Backup** before clearing data, moving devices, or replacing the app file.
