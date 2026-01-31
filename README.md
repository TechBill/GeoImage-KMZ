# GeoImage-KMZ

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS-4EAA25)
![License](https://img.shields.io/badge/License-Free--binary--distribution-orange)
![Release](https://img.shields.io/badge/Release-v2.0.0-6f42c1)

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
- Includes a **Paste Coordinates** button to quickly paste coordinates copied from Google Maps, Google Earth Pro, or QGIS
- Uses multiple control points to compute a best-fit alignment
- Exports a KMZ file that can be opened in Google Earth and other KMZ-compatible GIS tools
- The overlay can be adjusted using Google Earth’s transparency slider to visually compare old and modern features

The app uses an **affine (best-fit) transformation**. This means the image can be rotated, scaled, and skewed, but it is **not bent or rubber-sheeted**.

---

## Documentation

📘 **Full documentation:** See USER_GUIDE.md for detailed instructions, coordinate copy examples, and troubleshooting.

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
