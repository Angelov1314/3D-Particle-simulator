# Lotus Particle

An interactive 3D particle art installation built with Three.js, featuring a lotus flower model controlled by hand gestures via webcam. Set to ambient music, with real-time sculpting and visual customization tools.

## Features

- **Hand Gesture Control** — Uses MediaPipe Hands to let you sculpt and interact with particles using your webcam
- **3D GLB Model Loading** — Load any `.glb` model and explode/reconstruct it as a particle system
- **Real-time Sculpting** — Push, pull, and deform particles with an adjustable brush
- **Particle Presets** — Switch between visual styles (spiral, vortex, grid, noise, etc.)
- **Drag & Drop** — Drop a `.glb` file directly onto the canvas to load it
- **Music Player** — Built-in ambient audio player (Sakura Plains) with volume control
- **Fullscreen Mode** — UI fades out on idle; reappears on mouse movement
- **Color Customization** — Per-particle color and background color controls

## Usage

Just open `index.html` in a modern browser — no build step required.

```bash
# Serve locally (recommended for webcam access)
npx serve .
# or
python3 -m http.server
```

Allow webcam access when prompted. Use your hand in front of the camera to interact with the particle field.

## Controls

| Action | Description |
|--------|-------------|
| Hand gesture (webcam) | Sculpt and attract particles |
| Drag & drop `.glb` | Load a new 3D model |
| Side panel | Switch presets, adjust brush, change colors |
| `F` key | Toggle fullscreen |
| Music bar | Play/pause ambient track, adjust volume |

## Tech Stack

- [Three.js](https://threejs.org/) — 3D rendering and particle system
- [MediaPipe Hands](https://mediapipe.dev/) — Real-time hand tracking
- Native WebGL / WebAudio API
- Pure HTML + JavaScript, zero build tools
