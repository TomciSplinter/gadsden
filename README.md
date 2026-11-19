# GADSDEN

Static site: a scroll-scrubbed snake film that ends on the Gadsden flag, a short history of the flag (1751–1776), the mascot, and a join section.

## Deploy on Vercel
Import this repo in Vercel. No build step: framework preset **Other**, leave build command and output directory empty. `index.html` is served from the root.

## Files
- `index.html` — the whole page (styles, script and fonts are inline).
- `film/` — the film frames. `film.json` lists the packs; each `.webp` pack is an animated WebP the page splits into single frames. Desktop gets 900 frames at 1920×1080 (60 fps source), phones get 450 frames at 1200×1080.
- `assets/` — posters, storyboard stills, mascot layers, logo and favicon.

## To change
- X link: search `https://x.com/` in `index.html`.
- Film captions: the `.beat` blocks in `index.html`; `data-in` / `data-out` are scroll positions from 0 to 1.

Fonts: League Gothic and Libre Caslon Text (SIL Open Font License), embedded in `index.html`.
