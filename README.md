# Skill Videos — GitHub Pages build (v4)

Static site, no build step. Live at https://akib897.github.io/skill.videos/

## Update the existing repo (akib897/skill.videos)
Everything changed in this build, so replace the repo contents:
1. In the repo, delete the old `uploads/` and `assets/` folders (old filenames are no longer used) and `shader-toggle-scene.js` (no longer needed).
2. **Add file → Upload files**: drag in `index.html`, `signal-particles.html`, `support.js`, `image-slot.js`, `.nojekyll`, and the `assets/` folder.
3. Upload the `uploads/` videos a few at a time (GitHub caps each drag at 25 MB).
4. Commit. Pages redeploys in ~1 minute; hard-refresh (Cmd/Ctrl+Shift+R).

Or with git:
```
git clone https://github.com/akib897/skill.videos && cd skill.videos
git rm -rq uploads assets shader-toggle-scene.js
cp -R /path/to/publish/. .
git add -A && git commit -m "v4: kinetic Vimeo badge, headline word-fill" && git push
```

## Files
- `index.html` — the site (Skill Videos v4)
- `support.js`, `image-slot.js` — runtime
- `signal-particles.html` — iframe background for the pipeline section
- `assets/` — logo marks, AI tool logos, menu reel
- `uploads/` — hero, showreel, event, corporate, and the four multi-format clips
- `.nojekyll` — required so GitHub serves files and folders as-is

## Notes
- React loads from the unpkg CDN, so viewers need internet.
- Vimeo embeds stream from Vimeo.
