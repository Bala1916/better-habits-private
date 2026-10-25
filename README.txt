# Better Habits — Private Android Home-Screen App

## What this package does
- Lets you enter steps, tea/coffee cups, water, sleep, workout minutes, and daily habits manually.
- Keeps your records in this browser's local storage on this device.
- Includes a web app manifest and service worker so the app can be installed from HTTPS and cached for offline opening after its first successful load.
- Does not connect to Google Fit, Health Connect, or any account.

## Publish from your Android phone using GitHub
1. Open GitHub in Chrome and sign in.
2. Create a new repository, for example `better-habits-private`. If you want the repository itself to be public, remember that the website files will be public; your daily entries are not included in the repository.
3. Upload all five files from this folder to the repository root: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, and `icon-512.png`.
4. In the repository, open Settings -> Pages.
5. Under Build and deployment, choose Deploy from a branch; select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. Open the URL it shows.
7. In Chrome on Android, tap the three-dot menu -> Install app or Add to Home screen.
8. Open the installed app once while online. Then test it by enabling Airplane mode and reopening it.

## Privacy notes
- The app does not send your daily entries to a server. The static app files are served by GitHub Pages, but your records stay in the browser storage on this device.
- Browser storage is not the same as encrypted vault storage. Anyone with access to your unlocked phone/browser profile may be able to open the app.
- Do not clear Chrome site data if you want to keep your entries. Use the in-app Export Backup button regularly and keep the JSON backup somewhere private.
- Installing the PWA does not add a password lock. A true app lock would require additional native-app functionality or Android's own app-lock feature if available.
- If you previously used the standalone HTML file, its local records may not transfer to the hosted version because browser storage is scoped to the site. Export from the old version first if it contains data.
