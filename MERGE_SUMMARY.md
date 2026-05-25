# Merge Summary — PowerBI Stimulator Enterprise

## Task Completed
The uploaded files and the existing workspace enterprise files have been merged into one cohesive, additive system inside the `enterprise` folder.

## Main Decisions
- The richer uploaded enterprise interface from `index (1).html` was used as the final `index.html`.
- The existing workspace enterprise package supplied repository structure, security, privacy, governance, PWA and deployment assets.
- Original features were not removed; the final version is additive.

## Cleanups
- Removed Cloudflare challenge injection.
- Removed Cloudflare email-obfuscation dependency.
- Replaced hidden email anchors with direct mail links.
- Standardised naming to `PowerBI Stimulator Enterprise`.
- Updated service worker cache.
- Updated Content Security Policy to allow the free SheetJS CDN used for XLSX support.

## Final Output
Use the `enterprise` folder as the upload-ready project for GitHub, Cloudflare Pages, GitHub Pages, Netlify or other static hosting platforms.


## Tablet Navigation Rectification
A final tablet usability fix was added for the itel Vista Tab 30s and similar devices. The app now uses:

- a compact scroll-safe side rail on larger screens;
- a bottom horizontal navigation rail on tablet/mobile screens;
- hidden tooltips on touch layouts to avoid accidental overflow;
- `100dvh` viewport handling so Chrome mobile address bars do not hide menu items.
