# GeoImage-KMZ

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS-4EAA25)
![License](https://img.shields.io/badge/License-Free--binary--distribution-orange)
![Release](https://img.shields.io/badge/Release-v1.1-6f42c1)

---

## Overview

GeoImage KMZ is a lightweight, standalone desktop application designed for historical and exploratory map research. It helps you align scanned or photographed maps (plat maps, railroad maps, atlases, etc.) with modern geographic coordinates so they can be overlaid in Google Earth.

The app is intentionally simple and fast, focusing on research and field scouting rather than survey-grade GIS accuracy.

Available for macOS and Windows as ready-to-run applications. No installation or Python knowledge required.

---

## What the App Does

- Loads any scanned or photographed map image (PNG, JPG, TIFF, etc.)
- Displays the image in a fast pan/zoom viewer window
- Allows you to add control points by matching locations on the old map to real-world latitude/longitude coordinates
- Uses multiple control points to compute a best-fit alignment
- Exports a KMZ file that can be opened in Google Earth and other KMZ-compatible GIS tools
- The overlay can be adjusted using Google Earth’s transparency slider to visually compare old and modern features

The app uses an **affine (best-fit) transformation**. This means the image can be rotated, scaled, and skewed, but it is **not bent or rubber-sheeted**.

---

## What the App Is Best For

- Locating old houses, schools, cemeteries, churches, and mills
- Tracing abandoned roads and railroads
- Narrowing large search areas down to specific fields or ridges
- Historical research and metal-detecting site scouting

The output is intended to be **“close enough to trust,” not survey-accurate**.

---

## Important Limitations

- Google Earth cannot bend or warp images
- Even with many control points, the overlay remains a flat image
- Old maps often contain survey errors and paper distortion
- Section lines or borders may not line up perfectly everywhere

This behavior is expected and normal.

---

## How This Differs From QGIS

- **Google Earth (KMZ):** flat overlay only, fast and simple
- **QGIS:** can warp/bend images using advanced transformations

GeoImage KMZ is optimized for Google Earth use. Advanced GIS warping is intentionally left to tools like QGIS.

---

## Installation & Running the App

### macOS

1. Download `GeoImage_KMZ.app`
2. (Optional) Move it to your Applications folder
3. First launch:
   - Double-click the app
   - If macOS blocks it:
     - System Settings → Privacy & Security
     - Click **Open Anyway**
   - Or right-click the app → **Open**

This is a standard macOS security feature for downloaded apps.

### Windows

1. Download `GeoImage_KMZ.exe`
2. Move it to a permanent location
3. First launch:
   - Double-click the file
   - If SmartScreen appears:
     - Click **More info** → **Run anyway**

This is a standard Windows security feature for unsigned apps.

---

## How to Use

1. Launch GeoImage KMZ
2. Click **Load Image…** and select your map image
3. Pan and zoom to explore the map
4. Click **Add Point** and select matching locations
5. Enter latitude/longitude in decimal format
6. Add **4–8 points** for best results
7. Click **Generate KMZ…**
8. Open the KMZ in **Google Earth Pro** and adjust transparency

---

## Tips for Best Results

- Use stable landmarks: road intersections, bridges, creek bends
- Avoid features that change over time
- Add more points near your area of interest
- Expect slight drift away from control points

---

## Support & Contact

GeoImage KMZ is a free tool created for historical researchers, genealogists, and metal detecting enthusiasts.

If you find it useful, please consider supporting development:

- PayPal: https://www.paypal.com/paypalme/techbill
- Buy Me a Coffee: https://buymeacoffee.com/techbill

**Author:** Bill Fleming (TechBill)  
**GitHub:** https://github.com/TechBill

---

## License

GeoImage KMZ is provided **as-is** for personal and research use.

The application is distributed as a **free binary**. Source code is not currently published. Redistribution is permitted provided this README and author credit remain intact.

---

Thank you for using GeoImage KMZ.
