# Sablune

*sable + lune: sand and moonlight.* A tiny ASMR sand-and-glass game for the browser
and phones. Swipe along the glowing line to slice a block of layered pastel sand,
watch the slice crumble down a glass funnel into a jar, and build a little piece of
sand art, one slow breath at a time. 🎧 Best with headphones.

- No libraries and no asset files: one `index.html` with canvas and the Web Audio API
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
