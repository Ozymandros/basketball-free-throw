# Free Throw Fun

A kid-friendly 3D basketball free-throw game that runs entirely in the browser. Drag up to shoot, chase swishes, and build your streak.

![Tech](https://img.shields.io/badge/Three.js-r128-black)
![License](https://img.shields.io/badge/license-MIT-blue)

## Play

Open `index.html` in a modern browser, or serve the folder locally:

```bash
# Python
python -m http.server 8080

# Node (npx)
npx serve .
```

Then visit `http://localhost:8080`.

No build step or install required — the game loads [Three.js](https://threejs.org/) from a CDN.

## How to play

1. **Drag up** on the court to aim and set power (a yellow arc preview shows the shot path).
2. **Release** to shoot. Tiny drags cancel the shot.
3. Score to grow your **streak**; misses reset it. Your **best** streak is tracked on screen.
4. Toggle sound with the 🔊 button in the top-right.

Works with mouse and touch.

## Features

- Full 3D court, hoop, backboard, and textured basketball
- Drag-to-shoot aiming with trajectory preview
- Physics for gravity, floor bounces, rim, and backboard
- Swish detection, net ripple, confetti, and cheer messages
- Procedural Web Audio SFX (no sound files)
- Responsive full-screen canvas for desktop and mobile

## Project layout

```
basketball-free-throw/
├── index.html   # Scene, physics, input, UI, and audio (single file)
└── README.md
```

## Requirements

- A modern browser with WebGL (Chrome, Firefox, Edge, Safari)
- Network access on first load for the Three.js CDN (or host Three.js yourself)

## License

MIT — see [LICENSE](LICENSE).
