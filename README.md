# VRiot

**Exploring the convergence of VR and IoT: giving physical devices a spatial, embodied presence.**

VRiot is a WebXR sandbox for prototyping how connected objects (sensors, actuators, smart devices) could be seen, understood, and controlled through a spatial interface instead of a 2D dashboard or app. It's an early-stage exploration, not a finished product.

## Why

IoT interfaces are still mostly flat: toggles, sliders, charts on a screen. VR/XR gives physical devices a spatial presence, a location, a shape, a behavior you can walk around and interact with directly. VRiot is the testbed for that idea, built by [niceunderground](https://niceunderground.xyz).

## Status

🧪 **Early stage.** This repo currently holds the project scaffold (Vite + React + React Three Fiber + React Three XR wiring, HTTPS dev setup for WebXR). No experiments are published yet. Expect the structure and this README to change as prototypes land.

## Stack

- [React](https://react.dev) 19
- [Vite](https://vite.dev) 7
- [React Three Fiber](https://docs.pmnd.rs/react-three-fiber) — React renderer for Three.js
- [React Three XR](https://github.com/pmndrs/xr) — WebXR (VR/AR) session handling
- [Three.js](https://threejs.org)
- [vite-plugin-basic-ssl](https://github.com/vitejs/vite-plugin-basic-ssl) — local HTTPS, required by the WebXR device APIs

## Getting started

```bash
git clone https://github.com/niceunderground/VRiot.git
cd VRiot
npm install
npm run dev
```

The dev server runs over HTTPS (self-signed cert) since WebXR requires a secure context. Open it in a WebXR-capable browser, or on a headset browser pointed at your machine's local IP.

```bash
npm run build      # production build
npm run preview    # preview the build locally
npm run lint        # eslint
```

## Direction

Open questions this exploration is meant to answer:

- What does a "spatial dashboard" for IoT devices actually feel like, compared to a flat app?
- Can device state (on/off, sensor readings, alerts) be represented as spatial, embodied objects instead of UI widgets?
- Where does XR genuinely add value for controlling physical devices, and where is it just novelty?

---

Part of the [niceunderground](https://niceunderground.xyz) research practice — new media art, creative technology, experimental interfaces.
