# Daily AI/ML Brain Warm-Up

A self-contained Progressive Web App (PWA): a daily 5-question AI/ML quiz that
adapts to the topics you find tricky. Works fully offline once installed, and
saves your progress privately on your device.

## Files
- `index.html` — the whole app (HTML + CSS + JS, no dependencies)
- `manifest.webmanifest` — makes it installable as an app
- `sw.js` — service worker for offline use
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` — app icons

## Put it on your iPhone (GitHub Pages — free, ~3 min)

1. Create a free account at https://github.com (skip if you have one).
2. Install **GitHub Desktop** (https://desktop.github.com) — no terminal needed.
3. In GitHub Desktop: **File → Add Local Repository**, choose this `quiz-app`
   folder, then **Publish repository** (you can keep it public; it's just a quiz).
4. On github.com, open the new repository → **Settings → Pages** →
   under "Build and deployment", set **Source: Deploy from a branch**,
   **Branch: main / (root)**, click **Save**.
5. Wait ~1 minute, then refresh. Pages shows your live URL, like
   `https://YOURNAME.github.io/quiz-app/`.
6. On your **iPhone**, open that URL in **Safari** → tap the **Share** icon →
   **Add to Home Screen**. You now have an app icon that opens full-screen and
   works offline.

## Updating questions later
Edit `index.html` (the `BANK` object holds all questions). In GitHub Desktop,
**Commit** then **Push**. The live app updates within a minute. On the phone,
reopen the app (it refreshes when online). If you change files, bump the
`CACHE` version string in `sw.js` so the new version is picked up.
