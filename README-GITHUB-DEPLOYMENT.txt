ATTENDANCE APP — GITHUB PAGES DEPLOYMENT

Files included:
- index.html: client application with a visible Install App button and platform-specific help; installation banner hides after installation is detected or the app is opened in standalone mode.
- manifest.webmanifest: installable Progressive Web App metadata.
- sw.js: offline cache/service worker.
- icons/: app icons for supported devices.
- LICENCE ISSUER.html: original issuer page included from the source ZIP.

Deploy:
1. Extract this ZIP.
2. Upload all files and the icons folder to the root of a GitHub repository (keep the folder structure).
3. In GitHub, open Settings > Pages and publish from the main branch/root.
4. Open the published HTTPS GitHub Pages link. The Install App bar is visible at the top.
5. Android: use Chrome and tap Install App. iPhone/iPad: use Safari > Share > Add to Home Screen. Computer: use Chrome/Edge and tap Install App or the install icon in the address bar.

Important:
- A hosted HTTPS link is required for PWA installation and service workers.
- Browser/device policies control whether the native install prompt is offered. If it is not offered, the visible button shows device-specific instructions. The banner is hidden after the browser reports app installation or when the app is launched in standalone mode; some browsers may not expose installation status, especially for manual Add to Home Screen flows.
- This is a web app installation, not an app-store APK/EXE. The original application logic was retained; this package adds PWA installation support.
