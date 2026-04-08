# 3D Particle Simulator

![Demo](demo.png)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Three.js](https://img.shields.io/badge/Three.js-000000?logo=threedotjs&logoColor=white)](https://threejs.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An interactive 3D particle art installation featuring a lotus flower model controlled by hand gestures via webcam. Built with Three.js and MediaPipe -- no build tools required.

**[Live Demo](https://angelov1314.github.io/3D-Particle-simulator/)**

## Features

- **Hand Gesture Control** -- sculpt and interact with particles using your webcam via MediaPipe Hands
- **3D GLB Model Loading** -- load any `.glb` model and explode/reconstruct it as a particle system
- **Real-time Sculpting** -- push, pull, and deform particles with an adjustable brush
- **Particle Presets** -- switch between visual styles (spiral, vortex, grid, noise, etc.)
- **Drag & Drop** -- drop a `.glb` file directly onto the canvas to load it
- **Ambient Music** -- built-in audio player with volume control
- **Fullscreen Mode** -- UI fades on idle, reappears on mouse movement
- **Color Customization** -- per-particle color and background color controls

## Getting Started

Open `index.html` in a modern browser. For webcam access, serve locally:

```bash
npx serve .
# or
python3 -m http.server
```

Allow webcam access when prompted. Use your hand in front of the camera to interact with the particle field.

## Controls

| Action | Description |
|---|---|
| Hand gesture (webcam) | Sculpt and attract particles |
| Drag & drop `.glb` | Load a new 3D model |
| Side panel | Switch presets, adjust brush, change colors |
| `F` key | Toggle fullscreen |
| Music bar | Play/pause ambient track, adjust volume |

## Tech Stack

- [Three.js](https://threejs.org/) -- 3D rendering and particle system
- [MediaPipe Hands](https://mediapipe.dev/) -- real-time hand tracking
- WebGL / WebAudio API
- Pure HTML + JavaScript, zero build tools
