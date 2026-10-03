# Atelier — 3D Commercial Space Planner

A single-file, browser-based 3D space planner built with Three.js. Lay out a cafe, co-working space, boutique or restaurant, recolor everything with a brand color, check fire-egress paths, get a live cost estimate, and export a PDF layout sheet.

## Features

- 3D room (12 × 10 m) with raycast furniture placement and ghost preview
- 4 templates: Cafe, Co-work, Boutique, Restaurant
- 12 procedurally built furniture pieces (no external models)
- Brand color picker that recolors branded surfaces instantly
- Animated fire-egress paths with a pulsing exit marker
- Live capacity meter, density, and cost breakdown (delivery + contingency)
- PDF export of a 2D layout sheet and a cost quote (jsPDF)
- Perspective / top-down floor plan camera transition

## Run locally

No build step. Just open `index.html` in a modern browser (internet connection required for the CDN libraries).

If your browser blocks anything, serve the folder:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Deploy to GitHub Pages

1. Push this folder to a GitHub repo.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
4. Your site will be live at `https://<username>.github.io/<repo>/`.

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| 1–9 | Select furniture item |
| Esc | Deselect item |
| V | Toggle perspective / floor plan |
| F | Toggle fire egress |
| C | Toggle cost panel |

## Tech stack

Three.js 0.160, Tailwind CSS (CDN), jsPDF 2.5.1, Font Awesome 6.4, Google Fonts (Archivo, Manrope, JetBrains Mono).

## License

MIT
