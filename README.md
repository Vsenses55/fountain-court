# Light Show Series

Interactive Three.js light shows by Visual Senses. Each page has a series switcher in the top-left corner to move between shows.

| # | Show | Path |
|---|------|------|
| 01 | **Fountain Court**: splash-pad fountain with choreographed jets, LEDs and mist | `/` |
| 02 | **Light Tunnel**: glide through an endless, winding tunnel of LED arches | `/light-tunnel/` |

Live at **https://vsenses55.github.io/fountain-court/**

---

## 01 · Fountain Court

An interactive splash-pad fountain: a 7×7 floor grid of jets plus an outer ring of arcing jets, choreographed shows with pauses between them, LED lighting in blues, purples, pinks and greens, glowing mist, splash crowns, and realistic ripples on a wet reflective floor.

**Controls**

- Drag to orbit 360°, scroll or pinch to zoom
- Tap the plaza to fire the jets in a ripple from where you tap
- **Show**: jump to any of the 8 shows; **Loop** repeats the current one
- **Light**: switch LED palettes
- **Mist** / **Sound**: toggle fog effects and water sound
- **Orbit / Low / Top**: camera presets

## 02 · Light Tunnel

An endless tunnel of LED arches on the same backdrop, with the same bloom, mist and wet reflective path as Fountain Court. Arches recycle from behind you to the far end, so the tunnel never runs out.

**Controls**

- Drag to look around
- **Show**: 8 light shows (Color Wash, Chase, Arc Sweep, Spiral, Twinkle, Heartbeat, Split, Rainbow Road); **Loop** repeats the current one
- **Light**: LED palettes (the default "Tunnel" palette is sampled from the reference video)
- **Speed**: Stop / Slow / Medium / Fast. You can also scroll, use W / S or ↑ / ↓, or press Space to stop
- **Route**: Straight or Winding (gentle left and right bends, with the view leaning into the turns)
- **Mist** / **Sound**: haze and an ambient pad that changes chord with each show

---

## Files

```
index.html               Fountain Court (site home)
light-tunnel/index.html  Light Tunnel
.nojekyll                tells GitHub Pages to serve the files as-is
```

Each page is a single self-contained HTML file. Three.js r160 loads from the jsDelivr CDN through an import map, so there is no build step.

## Running it locally

Opening an `index.html` directly works for each show. To test the switcher links between shows, serve the folder:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Hosting on GitHub Pages

Repo **Settings → Pages → Build and deployment → Deploy from a branch → `main` / root**. The site will be at `https://vsenses55.github.io/fountain-court/`, with the tunnel at `/fountain-court/light-tunnel/`.

## Adding show No. 3

Add a folder such as `next-show/index.html`, then add a pill for it to the `.series` block in each page. Use `<span>` for the current page and `<a href="…">` for the others.
