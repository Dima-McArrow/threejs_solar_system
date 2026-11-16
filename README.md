# The Solar System · An Orbital Atlas

An interactive 3D model of the Solar System built with [Three.js](https://threejs.org/). The Sun and all eight planets sit in a single `index.html` file. There is no build step and nothing to install.

## Features

- The Sun, drawn with a glowing halo generated in code
- Eight planets with real surface textures, axial tilts, spin directions and relative orbital periods
- Rings around Saturn and Uranus, with concentric bands
- A starfield of 8,000 colored stars
- Orbit lines for every planet
- Camera controls via `OrbitControls`: rotate, zoom and pan
- Fallback colors if a planet texture fails to load or takes longer than 15 seconds
- Responsive layout that also works on mobile

> Sizes and distances are compressed so the whole system is easy to explore. They are not to scale.

## Getting Started

The page loads ES modules through an import map, so serve it over HTTP. Opening the file directly with `file://` won't work.

```bash
# Python
python3 -m http.server 8000

# or Node.js
npx serve .
```

Then open <http://localhost:8000> in your browser.

## Controls

| Action | Input       |
| ------ | ----------- |
| Rotate | Left click  |
| Zoom   | Scroll      |
| Pan    | Right click |

## Requirements

- A modern browser that supports WebGL and import maps
- An internet connection. Three.js (v0.180.0) loads from jsDelivr and planet textures load from [Solar System Scope](https://www.solarsystemscope.com/textures/)

## Project Structure

```
.
├── index.html   # Markup, styles and the whole Three.js scene
└── README.md
```

## Credits

- 3D rendering: [Three.js](https://threejs.org/)
- Planet textures: [Solar System Scope](https://www.solarsystemscope.com/textures/) (CC BY 4.0)
