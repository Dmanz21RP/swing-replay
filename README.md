# Swing Replay

Record golf swings, auto-tag P1–P8 with a still frame of each position, and replay them in slow motion with frame stepping, tempo ratio, drawing tools and side-by-side compare.

It's a single static page (`index.html`) with no build step. Swings are stored in the browser's IndexedDB on the device that recorded them; nothing is uploaded.

## Install on iPhone

1. Open the GitHub Pages URL in Safari.
2. Tap Share → Add to Home Screen.
3. Allow camera access the first time you record.

## Develop

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765. Camera access works on `localhost` and on the https Pages site.

When you change app files, bump `VERSION` in `sw.js` so installed copies pick up the update.
