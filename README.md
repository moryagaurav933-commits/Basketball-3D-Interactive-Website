# 🏀 Y68° — 3D Street Basketball Interactive Experience

<div align="center">

[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Three.js](https://img.shields.io/badge/Three.js-black?style=for-the-badge&logo=three.js&logoColor=white)](https://threejs.org/)
[![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)](https://greensock.com/gsap/)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/)

**An elevated, high-performance 3D interactive web application bridging cutting-edge 3D asset rendering, physics-based drag interactions, and modern liquid-glass aesthetics.**

[🌟 **Live Demo**](#-live-deployment) • [📖 **The Story Behind The Project**](#-the-journey--consistent-practice-to-the-next-level) • [⚡ **Features**](#-key-features) • [🛠️ **Tech Stack**](#️-tech-stack) • [🚀 **Getting Started**](#-getting-started)

</div>

---

## 🌟 The Journey — Consistent Practice to the Next Level

> *"Consistent, relentless practice isn't just about repetition — it's about pushing past comfort zones to unlock a higher caliber of craft."*

This project marks a personal milestone in my creative web development journey. Moving forward from traditional 2D web layouts and standard front-end design, my goal has been to master **3D asset-assisted web experiences** and elevate my work to an **upper level of polish and interactivity**.

Through dedicated daily practice with:
- **Spatial 3D Environments & WebGL rendering** with Three.js
- **Mathematical physics animations** (momentum, velocity decay, spherical drag, and inertia)
- **Cinema-grade scroll choreography** linking 3D space with DOM elements via GSAP ScrollTrigger
- **Liquid-glass refraction & distortion** using SVG turbulence filters and layered glassmorphism

This project represents that leap forward. It combines raw street basketball culture with futuristic, tactile interface design — proving that consistent practice turns complex 3D concepts into smooth, responsive real-world web apps.

---

## ⚡ Key Features

### 🏀 1. Interactive 3D Basketball with Real Physics
- **Draco-Compressed GLTF 3D Model**: High-fidelity basketball model loaded asynchronously with Google Draco decoders for lightning-fast asset delivery.
- **Physical Drag & Throw Momentum**: Users can click and flick or touch-drag the ball in full 3D space. When released, realistic momentum damping (`DAMPING = 0.94`) carries the spin naturally in the thrown direction before settling back into a smooth idle orbit.
- **ACES Filmic Tone Mapping & PMREM Reflections**: Rendered using high-performance tone mapping (`ACESFilmicToneMapping`) combined with `RoomEnvironment` PMREM generators, giving the leather ball realistic specular highlights, grain depth, and gritty court reflections.

### 📜 2. Cinematic Scroll-Driven Choreography
- **Section Waypoints**: As you scroll through the website, the 3D basketball smoothly transitions between coordinate waypoints (`hero` → `stats` → `how` → `footer`).
- **Depth Recession & Dynamic Parallax**: Custom easing (`easeInOut` + `lerp`) coupled with mathematical depth offsets (`depthOffset(y)`) so the ball recedes backwards into the z-plane as it travels down the page, delivering a true 3D spatial feel without obstructing readable content.

### 🔮 3. Liquid-Glass (Glassmorphism 2.0) UI
- **SVG Displacement Filter Distortion**: Multi-layer glass cards utilizing `<feTurbulence>` and `<feDisplacementMap>` to simulate organic refraction on hover and scroll.
- **3-Layer Depth Structure**: Cards feature distinct bend, face glow, and inset edge highlight layers for an authentic physical acrylic feel.
- **Micro-Interactions**: Pulse indicators, smooth avatar stack badges, hover lifts, and animated SVG vector strokes.

### 📱 4. Fully Responsive & Mobile-Optimized
- Handles touch events (`touchstart`, `touchmove`, `touchend`) with passive flag optimizations.
- Dynamic aspect ratio adjustment and pixel-ratio capping (`Math.min(devicePixelRatio, 2)`) to ensure high FPS on both high-end desktops and mobile devices.

---

## 🛠️ Tech Stack

| Category | Technology | Description |
| :--- | :--- | :--- |
| **Core 3D Engine** | [Three.js](https://threejs.org/) (r176) | WebGL scene, Perspective Camera, Ambient/Directional/Hemisphere Lighting, Mesh materials |
| **Asset Pipeline** | GLTFLoader + DRACOLoader | Compressed 3D GLB model parsing |
| **Animation Engine** | [GSAP](https://greensock.com/gsap/) + ScrollTrigger | Timeline choreography, entrance transitions, and scroll scrubbing |
| **Bundler & Tooling**| [Vite](https://vitejs.dev/) | Ultra-fast HMR and optimized production rollup builds |
| **Styling & Effects**| CSS3 + SVG Filters | Liquid glass aesthetics, Bebas Neue & Inter typography, noise overlays |
| **Deployment** | [Vercel](https://vercel.com/) / GitHub Pages | Continuous global edge delivery |

---

## 🚀 Getting Started

Follow these steps to run the project locally on your machine:

### Prerequisites
- [Node.js](https://nodejs.org/) (version 18 or higher recommended)
- `npm` or `pnpm` / `yarn`

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/moryagaurav933-commits/Basketball-3D-Interactive-Website.git
   cd Basketball-3D-Interactive-Website
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the local development server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) in your browser to view the interactive 3D site!

4. **Build for production:**
   ```bash
   npm run build
   ```
   The bundled production assets will be generated in the `dist/` directory.

5. **Preview production build:**
   ```bash
   npm run preview
   ```

---

## 🌐 Live Deployment

- **Live URL**: *(Deploying now...)*
- **GitHub Repository**: [https://github.com/moryagaurav933-commits/Basketball-3D-Interactive-Website](https://github.com/moryagaurav933-commits/Basketball-3D-Interactive-Website)

---

## 👨‍💻 Author

**Gaurav Morya**
- GitHub: [@moryagaurav933-commits](https://github.com/moryagaurav933-commits)
- Passionate about interactive 3D web experiences, creative frontend engineering, and game-inspired UI design.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE). Feel free to use it for learning, inspiration, and building your own 3D web journeys!
