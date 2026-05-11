# THE CHASE — Sixteen Wins. One Trophy.

An immersive WebGL scrollytelling experience following the journey to basketball's ultimate prize. Persistent Three.js scene, GSAP/ScrollTrigger-driven cinematic transitions, editorial typography.

## Run locally

The page loads `player.glb` over HTTP, so it must be served — opening the HTML directly via `file://` will fail.

```bash
# from inside this folder
python -m http.server 8000
```

Then open <http://localhost:8000/the-chase.html>.

## What's in the page

- **Scene 1: The Ball** — procedural basketball with PBR pebble texture and 4-seam topology
- **Section 02: By the Numbers** — animated stats reel with sparkline charts
- **Scene 2: The Contender** — basketball player GLB rising into frame
- **Sections 04.x: Data Blocks** — shot chart, doctrine quote, margin chart, bracket, eras radar
- **Scene 3: The Trophy** — drag-rotatable Larry O'Brien-style trophy with HDR-lit gold
- **Sections 05.x–06: Closing** — horizontal moments carousel, decade metrics, champions roll

## Tech stack

- [Three.js](https://threejs.org/) 0.160 (ES modules via importmap)
- [GSAP](https://gsap.com/) 3.12 + ScrollTrigger
- Polyhaven HDR for environment lighting
- UnrealBloom post-processing

## Credits

**3D basketball player model**: ["v0 Basketball Jump Shot Player Store"](https://sketchfab.com/3d-models/v0-basketball-jump-shot-player-store-8324d62b5eb64ccd8a597407578c85bd) by **TulioPortela**, licensed under [CC Attribution 4.0](https://creativecommons.org/licenses/by/4.0/). The model has been processed (split into a single figure, decimated, re-exported) for this project.

**HDR environment**: `studio_small_09_2k` from [Polyhaven](https://polyhaven.com), CC0.
