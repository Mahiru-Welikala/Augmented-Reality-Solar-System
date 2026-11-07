# Solar System AR

Marker-based WebAR (A-Frame + AR.js). Point the camera at the **Hiro marker** to see the sun, 4 planets, a moon and a rocket.

**Live link:** https://augment-reality-solar-system.netlify.app/

## What is in it
| Task | Where |
|---|---|
| Marker scene (5+ objects, many shapes, text) | plane, spheres, rings, box (moon), rocket, `<a-text>` |
| Animation (rotation + position) | planets + moon orbit (rotation), rocket floats (position) |
| 3D model (not the duck) | `rocket.glb` |
| Interaction | tap **Earth** = change colour, tap **Sun** = grow / shrink (bottom buttons do the same) |
| Status banner | green = marker found, red = marker lost |
| Hosting | HTTPS (Netlify) |

## Components (own code)
- `color-changer` - tap Earth (or its button), next colour
- `grow-toggle` - tap Sun (or its button), grow / shrink
- `marker-status` - banner text + colour

## Model credit
- `rocket.glb` - made by our group (built with Python + trimesh).
- Shapes: cylinder body, cone nose, sphere window, 3 box fins, cone flame.
- Licence: CC0 (public domain). Original work, no outside model used.

## Libraries
- A-Frame 1.4.2 (MIT)
- AR.js 3.4.5 (MIT)

## Run
1. VS Code > right-click `index.html` > Open with Live Server
2. Allow camera, show Hiro marker
3. Phone needs HTTPS (camera is blocked on plain http), so test the hosted link

## Host (HTTPS)
- Netlify Drop: drag the whole folder to app.netlify.com/drop
- or GitHub Pages: Settings > Pages > main branch

## Files
```
SolarSystemAR/
├── index.html
├── README.md
└── rocket.glb
```

## Hiro marker

The scene only shows when the camera sees the Hiro marker.

- Download: https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/hiro.png
- Print on A4 / Letter (black and white is fine), at least 10 cm wide.
- Keep it flat, in good light, fully in view.

1. Open the live link on your phone.
2. Allow camera.
3. Show the marker, wait 1-2 seconds.
4. Tap the Sun or Earth, or use the buttons at the bottom.
