# Solar System AR

Marker-based WebAR (A-Frame + AR.js). Point the camera at the **Hiro marker** to see the sun, 4 planets and a rocket.

link to view: https://augment-reality-solar-system.netlify.app/

## What is in it
| Task | Where |
|---|---|
| Marker scene (5+ objects, many shapes, text) | plane, spheres, rings, box (moon), rocket, `<a-text>` |
| Animation (rotation + position) | planets + moon orbit (rotation), rocket floats (position) |
| 3D model (not the duck) | `rocket.glb` |
| Interaction | tap **Earth: colour** button = earth colour change, tap **Sun: grow/shrink** button = sun grow / shrink |
| Status banner | green = marker found, red = marker lost |
| Hosting | HTTPS (see below) |

## Components (own code)
- `color-changer` - tap Earth button, colour changes of Earth
- `grow-toggle` - tap Sun button, the Sun will grow / shrink
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
- [https://augment-reality-solar-system.netlify.app/]

## Files
```
SolarSystemAR/
├── index.html
├── README.md
└── rocket.glb
---

## How to Get and Use the Hiro Marker

The Solar System only appears when the camera can see the **Hiro marker**.

### Download the marker

- Official Hiro marker (recommended):  
  https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/HIRO.jpg

- Alternative version (PNG):  
  https://raw.githubusercontent.com/AR-js-org/AR.js/master/data/images/hiro.png

### How to print it

1. Open one of the links above.
2. Print it on normal A4 or Letter paper (black & white is fine).
3. Make the printed marker at least 10–15 cm wide.
4. Keep the paper flat.

### How to use it

1. Open the project on your phone using an **HTTPS** link.
2. Allow camera access when asked.
3. Hold the printed Hiro marker in front of the camera.
4. Wait 1–2 seconds — the Solar System should appear on the marker.

### Tips for best results

- Use good lighting and avoid strong shadows on the marker.
- Keep the marker flat and fully visible to the camera.
- If the scene disappears, slowly move the marker back into view.
- Hold the phone steady for better tracking.

---
