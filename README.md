# ORBITA

A one-button browser arcade game. Your ship is locked to a ring around a dying star.
Tap to flip direction, hold to spin faster, collect crystals, dodge asteroids.

## Play

https://orbita-game.vercel.app

## Rules

- **Click / tap / space** — reverse your orbit direction instantly
- **Hold** — accelerate the rotation
- **Crystals** — pick them up for points; pick-ups within 2.4 s chain into a combo multiplier
- **Asteroids** — a pink arc appears on the ring where an incoming rock will cross it.
  That is your warning: be somewhere else, or flip past it.
- Score grows with survival time; difficulty ramps for ~75 seconds and then plateaus.
- Best score is kept in `localStorage`.

## Tech

Single static `index.html` — no build step, no dependencies. Canvas 2D, a fixed
900-unit design space scaled to the viewport, fixed-timestep-clamped loop,
pointer + keyboard input, `localStorage` for the record.

## Run locally

Just open `index.html`, or serve the folder:

```bash
python3 -m http.server 8080
```
