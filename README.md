<img width="1675" height="796" alt="image" src="https://github.com/user-attachments/assets/4f55c158-9fbc-4481-ab42-a3e0068c3219" />

# 3D Solar System

An interactive 3D solar system visualization built with Three.js. Explore the Sun and all eight planets with realistic procedural textures, orbital mechanics, and detailed planetary data.

## Features

- **3D Solar System** — Sun, Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune with accurate relative sizes and orbital distances
- **Procedural Textures** — Every planet has a unique procedurally generated surface texture (craters on Mercury, clouds on Venus, continents on Earth, bands on Jupiter, rings on Saturn, etc.)
- **Interactive Controls** — Orbit, pan, and zoom using mouse drag and scroll
- **Planet Info Panel** — Click any planet to view detailed stats (mass, diameter, temperature, gravity, moons, day length, description)
- **Fly-To Camera** — Smooth camera flyover to any planet with a single click
- **Moons** — Earth's Moon and Jupiter's four Galilean moons (Io, Europa, Ganymede, Callisto)
- **Asteroid Belt** — Decorative asteroid belt between Mars and Jupiter
- **Orbit Speed Control** — Adjust animation speed or pause the simulation
- **Starfield** — Thousands of randomly distributed stars

## Quick Start

Open `solar_system.html` in any modern browser (Chrome, Firefox, Edge recommended).

No build tools, no dependencies to install — the file loads Three.js from CDN via importmap.

```bash
git clone <repo-url>
cd <repo-directory>
# Open solar_system.html in your browser
```

Or simply open the file directly:

```bash
start solar_system.html
```

## Controls

| Action | Control |
|--------|---------|
| Orbit camera | Click and drag |
| Zoom | Scroll wheel |
| View planet info | Click on a planet |
| Fly to planet | Click planet → click "Fly To" button in info panel |
| Back to overview | Click "Back to Overview" button in info panel |
| Close info panel | Click ✕ button or press Escape |
| Adjust orbit speed | Drag the speed slider (top-right) |
| Pause/Resume | Click the pause button (top-right) |
| Reset camera | Click "Reset View" button (top-right) |

## Technical Details

- **Framework**: Three.js (r160) loaded from CDN via ES module importmap
- **Textures**: Procedurally generated on Canvas at runtime — no external image assets required
- **Rendering**: WebGL with ACES Filmic tone mapping
- **Scaled Model**:
  - 1 AU = 20 scene units
  - Planet sizes are proportional but exaggerated for visibility
  - Orbital periods are compressed for smooth animation

## Browser Support

Any browser with WebGL and ES module support:
- Chrome 61+
- Firefox 60+
- Safari 16.4+
- Edge 79+

## License

MIT
