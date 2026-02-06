# City Simulator 🏙️

A 3D interactive city simulator built with **Three.js** as part of the Computer Graphics course at NTNU, Norway.

## Demo

Open `index.html` in a browser to run the simulator.

## Features

- **3D City Environment** — Procedurally generated city with buildings, roads, bridges, streets, and terrain
- **Day/Night Simulation** — Directional light simulating sun movement across the sky with real-time shadow casting
- **Interactive GUI Controls** — Built with dat.GUI for real-time interaction:
  - Start/Reset simulation
  - Add, select, update, and delete buildings
  - Compute visibility and sky exposure analysis
  - Show light intensity heatmap
  - Save/Load scene (GLTF format)
- **Landmark Placement** — Place and select landmarks in the city
- **Light Intensity Visualization** — Heatmap overlay showing light distribution across the environment using chroma.js color scaling
- **Orbit Camera Controls** — Navigate the 3D scene with mouse (rotate, zoom, pan)

## Tech Stack

| Technology | Purpose |
|-----------|---------|
| [Three.js](https://threejs.org/) | 3D rendering engine |
| [dat.GUI](https://github.com/dataarts/dat.gui) | Interactive control panel |
| [Plotly.js](https://plotly.com/javascript/) | Data visualization |
| [Chroma.js](https://gka.github.io/chroma.js/) | Color scaling for heatmaps |
| [Perlin Noise](https://en.wikipedia.org/wiki/Perlin_noise) | Terrain generation |
| [Tween.js](https://github.com/tweenjs/tween.js) | Animation tweening |
| GLTF Loader/Exporter | Scene save & load |

## Project Structure

```
citySimulator-master/
├── index.html          # Entry point
├── js/
│   ├── main.js         # Core application logic (1100+ lines)
│   ├── three.js        # Three.js 3D library
│   ├── dat.gui.js      # GUI controls
│   ├── OrbitControls.js # Camera navigation
│   ├── perlin.js       # Perlin noise for terrain
│   ├── chroma.min.js   # Color scaling
│   ├── plotly-latest.min.js # Plotting
│   ├── Tween.js        # Animation
│   ├── GLTFLoader.js   # Scene loading
│   └── GLTFExporter.js # Scene exporting
├── assets/
│   ├── textures/       # Building, road, terrain textures
│   └── fonts/          # 3D text fonts
├── scenes/
│   └── scene.gltf      # Saved scene file
└── css/
    └── main.css        # Styling
```

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/ZeshanMubashir/Computer-Graphics.git
   ```
2. Open `index.html` in a web browser (use a local server for best results):
   ```bash
   npx serve .
   ```
3. Use the GUI panel on the right to interact with the city.

## Controls

| Action | Input |
|--------|-------|
| Rotate camera | Left mouse drag |
| Zoom | Scroll wheel |
| Pan | Right mouse drag |
| Select building | Click on building (enable "Select Building" in GUI) |

## Course

**Computer Graphics** — M.Sc. ICT - Simulation & Visualization, NTNU, Ålesund, Norway

## Author

**Zeshan Mubshir** — [Portfolio](https://zeshanmubashir.github.io) | [LinkedIn](https://www.linkedin.com/in/zeshanmubshir/)
