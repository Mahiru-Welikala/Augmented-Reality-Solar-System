# Solar System AR

Marker-based WebAR (A-Frame + AR.js). Point the camera at the **Hiro marker** to see the sun, 4 planets, a moon and a rocket.

**Live link:** _paste your Netlify / GitHub Pages link here_

## What is in it
| Task | Where |
|---|---|
| Marker scene (5+ objects, many shapes, text) | plane, spheres, rings, box (moon), rocket, `<a-text>` |
| Animation (rotation + position) | planets + moon orbit (rotation), rocket floats (position) |
| 3D model (not the duck) | `rocket.glb` |
| Interaction | tap **Earth** = colour change, tap **Sun** = grow / shrink (bottom buttons do the same) |
| Status banner | green = marker found, red = marker lost |
| Hosting | HTTPS (see below) |

## Components (own code)
- `color-changer` - tap Earth, next colour
- `grow-toggle` - tap Sun, grow / shrink
- `marker-status` - banner text + colour

## Model credit
- `rocket.glb` - made by our group (built with Python + trimesh).
- Licence: CC0 (public domain). Original work, no outside model used.

## Libraries
- A-Frame 1.3.0 (MIT)
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
