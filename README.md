# Skill Videos — internal review build

Static site. No build step.

## Publish on GitHub Pages
1. Create a repo (private is fine — Pages on private repos needs a paid plan; use public if unsure).
2. Upload the **contents of this folder** to the repo root (index.html must be at the top level).
3. Settings → Pages → Source: "Deploy from a branch" → Branch: `main` / `/ (root)` → Save.
4. Wait ~1 min. URL: `https://<user>.github.io/<repo>/`

## Files
- `index.html` — the site
- `support.js`, `shader-toggle-scene.js`, `image-slot.js` — runtime + canvas scenes
- `signal-particles.html` — iframe background for the pipeline section
- `assets/` — logos, menu reel
- `uploads/` — hero video, showreel, Event + Corporate samples (local MP4s)
- `.nojekyll` — required so GitHub serves files/folders as-is

## Notes
- React is loaded from unpkg CDN, so viewers need internet (fine for internal review).
- Vimeo embeds stream from Vimeo and are not in this folder.
- `Services.dc.html` is linked from the pricing note but does not exist yet — that link will 404.
