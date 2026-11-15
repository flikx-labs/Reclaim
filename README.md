# Reclaim — Mindful Habit Freedom & Clinical Urge Surfing

**Reclaim** is a zero-cloud, offline-first Progressive Web App (PWA) for habit cessation, neurobiological recovery tracking, and clinical urge surfing.

## Package Contents
- `index.html` — Complete application UI, CSS, clinical timelines, Web Audio synthesizer, and local storage engine (zero external JS dependencies).
- `manifest.json` — W3C Web App Manifest with Android, iOS, and Desktop installation metadata, maskable icons, and quick-launch app shortcuts.
- `sw.js` — Offline-first Service Worker (`reclaim-pwa-v2`) with navigation fallback and Stale-While-Revalidate asset/font caching.
- `icon.svg` — Scalable vector app icon.
- `icon-192.png` & `icon-512.png` — Raster PWA icons for Android/Chromium home screen and splash screen installation.
- `apple-touch-icon.png` — 180×180 iOS/iPadOS Home Screen icon.

## Deploying on GitHub Pages / Static Hosting
1. Create a new repository on GitHub (or any static host such as Cloudflare Pages, Vercel, or Netlify).
2. Upload all files from this archive (`index.html`, `manifest.json`, `sw.js`, `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, and `README.md`) to the root of your repository.
3. Open **Settings → Pages** in your GitHub repository.
4. Set **Source** to **Deploy from a branch** and select `main` (`/root`), then click **Save**.
5. Visit your live URL on mobile or desktop and click **Install** in the top bar (or **Share → Add to Home Screen** on iOS Safari).

## Privacy Architecture
100% of user data is stored locally on your device inside `localStorage` (`reclaim:v1`) with zero external database calls or telemetry. You can export and restore `.json` backups anytime from the **Settings** menu.
