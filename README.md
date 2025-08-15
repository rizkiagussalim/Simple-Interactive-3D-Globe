# 🌍 Interactive 3D Globe with GeoJSON Data

An interactive web application that displays a 3D globe with world city location data using Three.js and WebGL.

## ✨ Features

- **Realistic 3D Globe**: Earth with detailed satellite photo texture
- **Full Interactivity**: Mouse controls for rotation, zoom, and pan
- **City Locations**: Red dots marking important world cities
- **Information Popup**: Click on dots to see city names
- **Responsive**: Adapts to various screen sizes
- **Anti-aliasing**: Smooth and high-quality rendering

## 🚀 How to Use

1. **Open `index.html` file** in a modern browser that supports WebGL
2. **Navigation Controls**:
   - **Click & Drag**: Rotate globe
   - **Scroll**: Zoom in/out
   - **Right Click & Drag**: Pan view
3. **City Interaction**: Click on red dots to see city names

## 🛠️ Technologies Used

- **Three.js 0.160.0**: 3D graphics library for web
- **WebGL**: Hardware-accelerated 3D rendering
- **ES6 Modules**: Modern JavaScript with import/export
- **GeoJSON**: Standard geographic data format
- **HTML5 Canvas**: WebGL rendering surface

## 📁 Code Structure

### Scene Setup
- Three.js scene with ambient and directional lighting
- Perspective camera with 75° field of view
- WebGL renderer with anti-aliasing

### Globe Rendering
- Sphere geometry with 5 unit radius
- Earth texture from NASA Blue Marble
- Phong material for realistic lighting effects

### Geographic Data
Cities displayed:
- **Jakarta** (106.8456°E, 6.2088°S)
- **Tokyo** (139.6917°E, 35.6895°N)
- **New York** (74.0060°W, 40.7128°N)
- **London** (0.1278°W, 51.5074°N)
- **Sydney** (151.2093°E, 33.8688°S)
- **Cairo** (31.2357°E, 30.0444°N)
- **Rio de Janeiro** (43.1729°W, 22.9068°S)

### Interactivity
- **Raycasting**: 3D object click detection
- **OrbitControls**: Smooth camera controls
- **Popup System**: Display city information on click

## 🎨 Styling

- **Dark Theme**: Black background with white text
- **Info Box**: Information panel with transparency and border
- **Popup**: Modern and responsive tooltip styling
- **Font**: Inter font family for clean typography

## 📱 Responsiveness

- Adapts to browser window size
- High-DPI display support
- Touch-friendly controls for mobile devices

## 🔧 Configuration

### Orbit Controls
- **Damping**: 0.05 for smooth movement
- **Min Distance**: 6.5 units (maximum zoom)
- **Max Distance**: 50 units (minimum zoom)
- **Screen Space Panning**: Disabled for more natural control

### Lighting
- **Ambient Light**: 0.5 intensity for general illumination
- **Directional Light**: 1.0 intensity from position (5, 3, 5)

## 🌐 Dependencies

The application uses CDN for Three.js:
```html
<script type="importmap">
{
    "imports": {
        "three": "https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.module.js",
        "three/addons/": "https://cdn.jsdelivr.net/npm/three@0.160.0/examples/jsm/"
    }
}
</script>
```

## 📋 Browser Requirements

- **WebGL Support**: Browser must support WebGL
- **ES6 Modules**: Support for JavaScript modules
- **Modern Browser**: Chrome 61+, Firefox 60+, Safari 10.1+, Edge 16+

## 🌐 Live Demo

**Online Demo**: [https://rizkiagussalim.github.io/Simple-Interactive-3D-Globe](https://rizkiagussalim.github.io/Simple-Interactive-3D-Globe)

## 🚀 How to Run

1. Clone or download this repository
2. Open `index.html` file in a browser
3. Ensure internet connection is active (for loading earth texture)

## 🔮 Future Development

- [ ] Add more cities and data
- [ ] Implement search and filter
- [ ] Automatic rotation animation
- [ ] Day/night mode
- [ ] Screenshot export
- [ ] Mobile gesture support

## 📄 License

This project is open source and available for both personal and commercial use.

## 👨‍💻 Created By

Developed with ❤️ using Three.js and modern web technologies.

---

**Note**: Make sure your browser supports WebGL and ES6 modules to run this application optimally.
