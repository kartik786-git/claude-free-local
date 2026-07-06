# Clone & Run Prompt

Copy and paste the prompt below into your AI assistant to clone and run this solar system project:

---

**Prompt:**

Create a 3D solar system simulation using Three.js as a single HTML file. Include:

1. The Sun with an emissive glow effect and pulsing corona particles
2. All eight planets (Mercury through Neptune) with:
   - Procedurally generated surface textures (craters, clouds, bands, etc.)
   - Realistic orbital mechanics (different speeds, distances, tilts)
   - Saturn's rings
   - Earth's Moon and Jupiter's four Galilean moons
3. Interactive features:
   - OrbitControls for camera (drag to orbit, scroll to zoom)
   - Click any planet to show an info panel with stats (mass, diameter, temperature, gravity, moons, day length, description)
   - Smooth fly-to camera animation when clicking "Fly To" button
   - Back to overview button
   - Orbit speed slider and pause/resume
   - Reset view button
4. A starfield background, orbit ring paths, decorative asteroid belt
5. Hover tooltip showing planet name, distance, and orbital period

The output should be a single `solar_system.html` file that:
- Uses Three.js r160 from CDN via importmap
- Has all textures generated procedurally in Canvas (no external images)
- Uses modern ES modules
- Works when opened directly in any modern browser

**File structure:**
```
/
├── solar_system.html   ← single self-contained HTML file
├── README.md           ← project documentation
└── CLONE_PROMPT.md     ← this prompt file
```

**To run:**
Simply open `solar_system.html` in your browser. No build tools, no npm install, no server required.
