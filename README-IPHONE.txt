FAMILY TIME LEDGER — IPHONE INSTALL EDITION
============================================

Important: this is an installable web app (PWA). iPhone requires the app files to be served from an HTTPS website before Safari can add it to the Home Screen. The app's records still stay in local browser storage on the iPhone; this does not add accounts or cloud syncing.

FILES
- index.html: the app
- manifest.webmanifest: install metadata
- service-worker.js: offline caching after the first load
- icon-192.png and icon-512.png: app icons

EASIEST FREE PUBLISHING OPTION: GITHUB PAGES
1. On a computer, sign in to GitHub or create a free account.
2. Create a new repository. For privacy, note that GitHub Pages on a free personal account generally requires a public repository; don't put private data in this repository. These files contain app code only, not your logs.
3. Upload all five app files from this folder to the repository's root.
4. In the repository, open Settings → Pages. Choose deploy from a branch, select the main branch and root folder, then save.
5. Wait for GitHub Pages to publish the HTTPS site.
6. On your iPhone, open the published HTTPS address in Safari.
7. Tap Share → Add to Home Screen. If offered, enable “Open as Web App”, then tap Add.
8. Open Family Time from the new Home Screen icon. Load it once while online so the offline cache can install. Then test airplane mode.

LOCAL DATA / BACKUPS
- Records are stored in Safari's local website storage on that iPhone, not on GitHub.
- Home Screen web app storage is separate from other browser/device storage; do not expect old desktop entries to appear automatically.
- Use the app's Backup data button regularly and keep the exported JSON somewhere safe.
- Clearing Safari website data or removing site data may erase records. A backup is essential.
- The service worker caches the app so it can launch offline after the first successful online visit. The app's data does not sync across devices.

ALTERNATIVE
If you don't want to publish the app files on a website at all, you can keep using the standalone HTML file on a computer, but a proper iPhone Home Screen web-app install needs an HTTPS origin. A native App Store app would require a separate build and signing/distribution process.
