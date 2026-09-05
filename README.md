# Skill Videos — internal review build

Static site, no build step. Upload the CONTENTS of this folder to the repo root.

## Update an existing GitHub Pages repo
1. In the repo, click **Add file → Upload files**.
2. Drag in `index.html` (and `support.js` if you have not uploaded it before).
3. Commit. Pages redeploys in ~1 minute; hard-refresh the live URL (Cmd/Ctrl+Shift+R).

Only `index.html` changed in this export — the videos, logos and helper scripts in
`uploads/` and `assets/` are unchanged, so you do not need to re-upload them.

## First-time setup
1. Upload everything inside this folder (videos go one at a time — GitHub caps each
   drag at 25 MB and the four clips total ~48 MB).
2. Settings → Pages → Deploy from a branch → `main` / `/ (root)`.

## Files
- `index.html` — the site
- `support.js`, `shader-toggle-scene.js`, `image-slot.js` — runtime + canvas scenes
- `signal-particles.html` — iframe background for the pipeline section
- `assets/` — logos, menu reel
- `uploads/` — hero-bg.mp4, showreel.mp4, sample-event.mp4, sample-corporate.mp4
- `.nojekyll` — required so GitHub serves files and folders as-is

## Notes
- React loads from the unpkg CDN, so viewers need internet. Fine for internal review.
- Vimeo embeds stream from Vimeo and are not in this folder.
- Links that pointed at pages we have not built yet (Services, Studio, Work) now jump
  to the relevant section on this page instead of 404ing.
