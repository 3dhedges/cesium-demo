# Cesium Lower Manhattan + CitiBike Demo

This demo showcases CesiumJS with:
- **Global OSM Buildings** and **World Terrain** from Cesium ion
- A **3D Tiled Dataset** of Lower Manhattan (Cesium ion asset #3806843)
- A **GeoJSON Footprint of Manhattan** used to clip OSM buildings (hidden from view)
- **CitiBike NYC live station data** (station info + real-time availability)

The map flies to Lower Manhattan and overlays live CitiBike stations as clickable bike icons.

---

## Live Demo
[▶ View on GitHub Pages](https://3dhedges.github.io/cesium-demo/)  

---

## Running Locally

Cesium uses dynamic ES modules and fetch requests, which require serving over HTTP.
If you simply open `index.html` with `file://`, the data will not load.

1. Clone or download this repository.
2. In the project folder, start a simple HTTP server:
   - **Python 3**: `python -m http.server 8000`
   - **Node.js**: `npx serve`
3. Open your browser to: [http://localhost:8000](http://localhost:8000)

---

## Cesium ion Access Token
The 3D Tiled textured buildings and the Manhattan footprint polygon layers are hosted in the account associated with the provided Cesium ion acces token.
To use this application in your own hosted environment, download these assets and host them in your own Cesium ion account.
