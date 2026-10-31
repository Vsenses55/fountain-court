# Fountain Court

An interactive Three.js splash-pad fountain: a 7×7 floor grid of jets plus an outer ring of arcing jets, choreographed shows with pauses between them, LED lighting in blues, purples, pinks and greens, glowing mist, splash crowns, and realistic ripples on a wet reflective floor.

## Controls

- Drag to orbit 360°, scroll or pinch to zoom
- Tap the plaza to fire the jets in a ripple from where you tap
- **Show**: jump to any of the 8 shows; **Loop** repeats the current one
- **Light**: switch LED palettes
- **Mist** / **Sound**: toggle fog effects and water sound
- **Orbit / Low / Top**: camera presets

## Files

- `index.html`: the whole experience (Three.js r160 loaded from a CDN via import map). There are no other files.

## Running it locally

Open `index.html` in a browser. If your browser blocks it from `file://`, serve the folder instead:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Hosting on GitHub Pages

Repo **Settings → Pages → Build and deployment → Deploy from a branch → `main` / root**. The site will be at `https://<username>.github.io/fountain-court/`.
