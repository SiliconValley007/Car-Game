# NITRO

A single-file HTML5 Canvas endless lane-racing game. Dodge traffic, chain near-misses, and chase your high score.

## Play

Open `index.html` in any modern browser — no build step, no dependencies, no server required.

> Live scoring, speed ramp-up, and sound use the Web Audio API and `localStorage` for high scores; both degrade gracefully if unavailable (e.g. `file://` privacy restrictions in some browsers).

## Controls

| Action | Key |
|---|---|
| Move left | `←` / `A` |
| Move right | `→` / `D` |
| Pause / Resume | `Esc` / `P` |
| Start / Restart | `Enter` / click |

## Features

- Procedural 3-lane traffic with adaptive spawn gaps and difficulty ramp
- Near-miss scoring with combo multiplier
- Persistent high score (`localStorage`)
- Lane-change bank animation, particle effects, screen shake, engine audio
- Responsive canvas (resizes to viewport, capped device-pixel-ratio for perf)
- `prefers-reduced-motion` support (disables shake/particles)

## Project structure

Single file: `index.html` (HTML + CSS + JS, no external assets or dependencies).

## Browser support

Any browser with Canvas 2D + Web Audio API support (all current Chrome, Firefox, Edge, Safari). Audio and high-score persistence are optional-fail — the game runs without them.
