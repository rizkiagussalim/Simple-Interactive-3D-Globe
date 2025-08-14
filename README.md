# 🌍 Interactive 3D Globe with GeoJSON Data

Sebuah aplikasi web interaktif yang menampilkan globe 3D dengan data lokasi kota-kota dunia menggunakan Three.js dan WebGL.

## ✨ Fitur

- **Globe 3D Realistis**: Bumi dengan tekstur foto satelit yang detail
- **Interaktivitas Penuh**: Kontrol mouse untuk rotasi, zoom, dan pan
- **Lokasi Kota**: Titik-titik merah yang menandai kota-kota penting dunia
- **Popup Informasi**: Klik pada titik untuk melihat nama kota
- **Responsif**: Menyesuaikan dengan berbagai ukuran layar
- **Anti-aliasing**: Render yang halus dan berkualitas tinggi

## 🚀 Cara Menggunakan

1. **Buka file `index.html`** di browser modern yang mendukung WebGL
2. **Kontrol Navigasi**:
   - **Klik & Drag**: Putar globe
   - **Scroll**: Zoom in/out
   - **Klik kanan & Drag**: Geser view
3. **Interaksi dengan Kota**: Klik pada titik merah untuk melihat nama kota

## 🛠️ Teknologi yang Digunakan

- **Three.js 0.160.0**: Library 3D graphics untuk web
- **WebGL**: Hardware-accelerated 3D rendering
- **ES6 Modules**: Modern JavaScript dengan import/export
- **GeoJSON**: Format data geografis standar
- **HTML5 Canvas**: Rendering surface untuk WebGL

## 📁 Struktur Kode

### Setup Scene
- Scene Three.js dengan lighting ambient dan directional
- Camera perspective dengan field of view 75°
- WebGL renderer dengan anti-aliasing

### Globe Rendering
- Sphere geometry dengan radius 5 unit
- Tekstur bumi dari NASA Blue Marble
- Material Phong untuk efek lighting realistis

### Data Geografis
Kota-kota yang ditampilkan:
- **Jakarta** (106.8456°E, 6.2088°S)
- **Tokyo** (139.6917°E, 35.6895°N)
- **New York** (74.0060°W, 40.7128°N)
- **London** (0.1278°W, 51.5074°N)
- **Sydney** (151.2093°E, 33.8688°S)
- **Cairo** (31.2357°E, 30.0444°N)
- **Rio de Janeiro** (43.1729°W, 22.9068°S)

### Interaktivitas
- **Raycasting**: Deteksi klik pada objek 3D
- **OrbitControls**: Kontrol kamera yang smooth
- **Popup System**: Menampilkan informasi kota yang diklik

## 🎨 Styling

- **Dark Theme**: Background hitam dengan teks putih
- **Info Box**: Panel informasi dengan transparansi dan border
- **Popup**: Tooltip dengan styling modern dan responsive
- **Font**: Inter font family untuk tipografi yang bersih

## 📱 Responsivitas

- Menyesuaikan dengan ukuran window browser
- High-DPI display support
- Touch-friendly controls untuk perangkat mobile

## 🔧 Konfigurasi

### Orbit Controls
- **Damping**: 0.05 untuk gerakan yang smooth
- **Min Distance**: 6.5 unit (zoom maksimal)
- **Max Distance**: 50 unit (zoom minimal)
- **Screen Space Panning**: Disabled untuk kontrol yang lebih natural

### Lighting
- **Ambient Light**: 0.5 intensity untuk pencahayaan umum
- **Directional Light**: 1.0 intensity dari posisi (5, 3, 5)

## 🌐 Dependencies

Aplikasi menggunakan CDN untuk Three.js:
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

- **WebGL Support**: Browser harus mendukung WebGL
- **ES6 Modules**: Support untuk JavaScript modules
- **Modern Browser**: Chrome 61+, Firefox 60+, Safari 10.1+, Edge 16+

## 🌐 Live Demo

**Demo Online**: [https://rizkiagussalim.github.io/interactive-3d-globe](https://rizkiagussalim.github.io/interactive-3d-globe)

## 🚀 Cara Menjalankan

1. Clone atau download repository ini
2. Buka file `index.html` di browser
3. Pastikan koneksi internet aktif (untuk loading tekstur bumi)

## 🔮 Pengembangan Selanjutnya

- [ ] Tambah lebih banyak kota dan data
- [ ] Implementasi search dan filter
- [ ] Animasi rotasi otomatis
- [ ] Mode malam/siang
- [ ] Export screenshot
- [ ] Mobile gesture support

## 📄 Lisensi

Proyek ini open source dan tersedia untuk penggunaan pribadi maupun komersial.

## 👨‍💻 Dibuat Oleh

Dikembangkan dengan ❤️ menggunakan Three.js dan teknologi web modern.

---

**Note**: Pastikan browser Anda mendukung WebGL dan ES6 modules untuk menjalankan aplikasi ini dengan optimal.
