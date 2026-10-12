# ReelForge AI

A free, browser-based reel planner and editor. No account, no API key, no server.

## What it does
- Reel wizard, local template-based script generator (not an AI model), hook library, scene planner
- Paste your own script and split it into scenes
- Captions and hashtags from a built-in keyword list (not live trends)
- Video editor: upload images/videos, text overlays, title/end cards, your own audio, 9:16 preview
- Export on your device (MP4 if your browser can encode it, otherwise WebM), 540x960
- Projects, favorites and settings are saved in the browser (localStorage). Editor media (images, video, audio) is saved in IndexedDB on this device. Clearing browser data removes everything. Backup/Restore covers projects, favorites and settings, not media files.

## Also included
- Social Tools: title, description and call-to-action generators (templates), thumbnail creator (PNG), content calendar (planner only)
- Installable web app (PWA): manifest, icons, service worker. Open the site over HTTPS and use "Install app" or "Add to Home screen".

## Not included
Accounts, cloud database and storage (planned: Cloudflare Workers, D1, R2), real AI generation, automatic subtitles from speech, publishing to social platforms, 720p/1080p export.

## Deploy on GitHub Pages
1. Create a new public repository and upload `index.html`, `README.md` and `.nojekyll` to the root.
2. Repository Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. Open `https://<your-username>.github.io/<repo-name>/` after a minute or two.

## Deploy on Cloudflare Pages (alternative)
Connect the repository, leave the build command empty, set the output directory to `/`.
