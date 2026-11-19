# GADSDEN

Static site: a scroll-scrubbed snake film that ends on the Gadsden flag, a short history of the flag (1751–1776), Alon (the mascot), and a join section.

Alon's parts of the page:
- He peeks into the final flag frame of the film.
- **Tale of the tape** card: Alon follows the pointer, blinks, and says a line with a rattle sound when tapped.
- **Alon was there**: a film strip of history scenes that slides sideways as you scroll.
- **Shirt maker**: type text, Alon wears it, save as PNG.
- The arena loop plays behind Join.

## Deploy on Vercel
Import this repo in Vercel. No build step: framework preset **Other**, leave build command and output directory empty. `index.html` is served from the root.

## Files
- `index.html` — the whole page (styles, script and fonts are inline).
- `film/` — the film frames. `film.json` lists the packs; each `.webp` pack is an animated WebP the page splits into single frames. Desktop gets 900 frames at 1920×1080 (60 fps source), phones get 450 frames at 1200×1080.
- `assets/` — posters, storyboard stills, mascot layers, logo and favicon.
- `assets/alon/` — Alon's rig (`alon-rig.webp` with a blank shirt + `alon-rig.json` for lens shapes and the shirt print area), peek image, history scenes, arena loop video and poster.

## To change
- X link: search `https://x.com/` in `index.html`.
- Film captions: the `.beat` blocks in `index.html`; `data-in` / `data-out` are scroll positions from 0 to 1.
- Alon's lines when tapped: the `LINES` list in the last script in `index.html`.
- Shirt ideas: the `.chips` buttons; `data-text` uses `/` for line breaks.

Fonts: League Gothic, Libre Caslon Text and Anton (SIL Open Font License), embedded in `index.html`.
