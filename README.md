# KIMI — GRIDO1 Racing Systems

A one-page driver site for **Kimi Antonelli**, driver_012 of GRIDO1 Racing Systems.

**Live:** https://nitingo17.github.io/kimi-grido1/

## What this is

A single self-contained `index.html` — no build step, no framework, no bundler.
Three.js and Lenis are the only external code (pulled through an import map);
the spring solver, the shared ticker, the scroll triggers, the text reveals, the
sticky stack, the circuit trace, the halftone, the chequered dissolves, the
contour backdrops and the loader are all written by hand.

Five blocks: the hero (a WebGL depth-parallax portrait with a helmet worn over
it), *the season so far* (a 2560x1440 halftone circuit map with a 6-second lap),
*from karts to F1* (the career timeline), *from the paddock*, and the footer.

## Assets

The page loads its images, textures and the Draco-compressed helmet model at
runtime from `https://storage.getlayers.ai/assets/kimi-04a9449ab2/`. That bucket
is third-party; if it is unavailable the page shows a banner naming the URL that
failed, and the loading veil holds at 70%.

## Run locally

Open `index.html` over HTTP (e.g. `python3 -m http.server`); ES module imports
do not work from `file://`.
