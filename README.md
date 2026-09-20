# TOWER-01 — playable build

A glass-themed tower defence. This repo holds **only the built game**: one
self-contained HTML file, published by GitHub Pages so playtesters have a single
link that is always the newest build.

**Play it:** https://shearinnick-code.github.io/tower-01-play/

The source lives elsewhere and is not part of this repo.

## For playtesters

Play until you win, lose, or get bored — then press **SAVE RUN** on the top edge
of the board. It saves a small file of every decision you made, which is what
the design work reads. You can press it at any point, not only at the end; if
something strange happens on wave 23, save it right then.

Nothing personal is recorded. The file contains the map you played, where you
put your towers, what you upgraded and when, and what the waves did back.

## Deploying a new build

From the game's source repo:

    npm run artifact
    cp dist/tower-01.html ../tower-01-play/index.html
    cd ../tower-01-play && git add -A && git commit -m "build <sha>" && git push

Pages picks it up within a minute. The link never changes, so testers get the
new build on their next reload without being told anything.
