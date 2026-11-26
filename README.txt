DELIVERY MESSENGER 2.0
Upload all seven files in this folder to the ROOT of the existing GitHub Pages repository, replacing index.html, manifest.webmanifest and sw.js:
- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png
- icon-maskable-512.png
- README.txt (optional)

PWA notes:
- HTTPS is required; GitHub Pages provides it.
- Chrome on Android should offer Install app when manifest, icons and service worker are available.
- If Chrome still only offers Create shortcut, use that; the app remains usable.
- After deployment, close the app and reopen. If old assets remain cached, close Chrome tabs for the site and reload; service worker cache version is v2.

Local storage:
- Platform, merchant, language and saved custom message templates are stored in localStorage on that device/browser.
- Recipient phone numbers are not stored.
- Clearing browser site data removes these preferences.

Messaging:
- WhatsApp and SMS are opened with a prefilled message. User reviews and sends manually.
- No integration with courier platform APIs and no automated sending.
