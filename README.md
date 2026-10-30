# Sablune

*sable + lune: sand and moonlight.* A tiny ASMR sand-and-glass game for the browser
and phones. Swipe along the glowing line to slice a block of layered pastel sand,
watch the slice crumble down a glass funnel into a jar, and build a little piece of
sand art, one slow breath at a time. 🎧 Best with headphones.

- No libraries: the whole game is one `index.html` with canvas and the Web Audio API
  (the icons, manifest and service worker are only there so it can be installed and played offline)
- Every sound (slice scrape, crunchy grains, settling sand, chimes, cork pop, glass clink) is synthesized live
- A breathing guide (4s in / 4s out) glows around the block; cutting on the out-breath is a "calm" cut
- Grains keep the colors of the layer they came from and pile up into sand-art layers
- Fill the jar, cork it and keep it on your shelf; nothing to fail

## Play locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Install on a phone

Sablune is a small web app: open it in Safari (iPhone) or Chrome (Android) and choose
**Share → Add to Home Screen** / **Install app**. It opens full screen and works offline.

## Hosting on GitHub Pages

Everything Pages needs is in this folder: `index.html`, `manifest.webmanifest`, `sw.js`,
`icons/`, `og-image.jpg` (the share preview) and `.nojekyll`. To publish:

1. Create a GitHub repository named `sablune` and push `main`.
2. Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.
3. The game appears at `https://helavika.github.io/sablune/`.

The share-preview tags in `index.html` point at that address; change them if the repo
or account name is different. After changing the game, bump `CACHE` in `sw.js` so
installed copies pick up new icons.
