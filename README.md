# Crumble

A tiny kinetic-sand ASMR game for the browser and phones. Swipe along the dotted
line to slice the sand block, watch the slice crumble into a pile, and listen to
the crunch. 🎧 Best with headphones.

- No libraries and no asset files: one `index.html` with canvas and the Web Audio API
- Every sound (slice scrape, crunchy grains, settling sand, chimes) is synthesized live
- Sand grains keep the colors of the layer they came from and roll down the pile
- Precision scoring (Perfect / Great / Good) with combos; nothing to fail

## Play locally

Open `index.html` in a browser, or serve the folder:

```sh
python3 -m http.server 8000
```

then visit http://localhost:8000.
