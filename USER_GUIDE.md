# GeoImage KMZ – User Guide

---

## Overview

GeoImage KMZ is a lightweight, standalone desktop application designed for historical and exploratory map research. It helps you align scanned or photographed maps (plat maps, railroad maps, atlases, aerials, etc.) with modern geographic coordinates so they can be overlaid in Google Earth and other KMZ-compatible tools.

The app is intentionally simple and fast, focusing on research and field scouting rather than survey‑grade GIS accuracy.

Available for macOS and Windows as ready‑to‑run applications. No installation or Python knowledge required.

---

## What the App Does

- Loads any scanned or photographed map image (PNG, JPG, TIFF, BMP, GIF, etc.)
- Displays the image in a fast pan/zoom viewer window
- Allows you to add control points by matching locations on the old map to real‑world latitude/longitude coordinates
- Uses multiple control points to compute a best‑fit alignment
- Exports a KMZ file that can be opened in Google Earth and other KMZ‑compatible GIS tools
- The overlay can be adjusted using Google Earth’s transparency slider to visually compare old and modern features

The app uses an **affine (best‑fit) transformation**. This means the image can be rotated, scaled, and skewed, but it is **not bent or rubber‑sheeted**.

---

## What the App Is Best For

- Locating old houses, schools, cemeteries, churches, and mills
- Tracing abandoned roads and railroads
- Narrowing large search areas down to specific fields or ridges
- Historical research and metal‑detecting site scouting

The output is intended to be **“close enough to trust,” not survey‑accurate**.

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

1. Download **GeoImage_KMZ.app**
2. (Optional) Move the app to your Applications folder
3. First‑time launch:
   - Double‑click the app
   - If macOS blocks it:
     - System Settings → Privacy & Security
     - Click **Open Anyway**
   - Or right‑click the app → **Open**

This is a standard macOS security feature for downloaded applications.

---

### Windows

1. Download **GeoImage_KMZ.exe**
2. Move it to a permanent location
3. First‑time launch:
   - Double‑click the file
   - If SmartScreen appears:
     - Click **More info** → **Run anyway**

This is a standard Windows security feature for unsigned applications.

---

## How to Use the App

1. Launch **GeoImage KMZ**
2. Click **Load Image…** and select your old map image
3. Pan and zoom to explore the map
4. Click **Add Point** and select matching locations
5. Enter latitude/longitude in **decimal format**
6. Add **4–8 control points** for best results
7. Click **Generate KMZ…**
8. Open the KMZ in **Google Earth Pro** and adjust transparency

---

## Tips for Getting Good Results

### Choosing Control Points

Use stable landmarks that exist on both the old map and modern imagery:
- Road intersections (especially T‑junctions)
- Bridge locations
- Creek bends and stream junctions
- Building corners (if the building still exists)
- Property or section corners

Avoid features that change over time:
- Tree lines
- Field edges
- Shorelines
- Railroad tracks that may have been removed

---

### How Many Points?

- **Minimum:** 3 points (required)
- **Recommended:** 4–8 points
- **More than 8:** diminishing returns

Add more points near your area of interest for better local accuracy.

---

## Getting Coordinates

### Google Earth Pro

1. Click **Add Placemark** (yellow pushpin)
2. Drag the pin to the desired location
3. Copy the latitude and longitude from the placemark dialog
4. Paste into GeoImage KMZ (decimal format)

### Google Maps

1. Right‑click a location
2. Click the coordinates shown
3. Paste into GeoImage KMZ

**Decimal format required:**  
`38.627003, -90.199402`

---

## Working With PLSS‑Based Maps

If your map shows **Township, Range, and Section** information:

- Use PLSS overlays in Google Earth Pro
- Match section corners from the old map to PLSS grid corners
- This greatly speeds up coordinate discovery

Search for:
- “PLSS KML overlay Google Earth”
- State or county GIS PLSS overlays
- BLM PLSS data

---

## Rotation Notes

- Use rotation buttons to fix sideways or upside‑down scans
- **Rotating clears all control points**
- Always rotate **before** adding points

---

## Troubleshooting

### Overlay Doesn’t Line Up Perfectly
This is normal due to map distortion and survey inaccuracies. Aim for best local accuracy near your area of interest.

### Points Disappeared
Points are cleared when rotating the image. Save points frequently using **Save Points…**.

### KMZ Won’t Open
- Use **Google Earth Pro** (desktop)
- Ensure the file ends with `.kmz`

---

## System Requirements

### macOS
- macOS 10.13 (High Sierra) or newer
- Works on Intel and Apple Silicon

### Windows
- Windows 10 or 11 (64‑bit)

### Both
- Google Earth Pro (free)
- Recommended: 4 GB RAM or more

---

## Support & Contact

GeoImage KMZ is a free tool for historical researchers, genealogists, and metal‑detecting enthusiasts.

Support development:
- PayPal: https://www.paypal.com/paypalme/techbill
- Buy Me a Coffee: https://buymeacoffee.com/techbill

**Author:** Bill Fleming (TechBill)  
**GitHub:** https://github.com/TechBill

---

## License & Credits

GeoImage KMZ is provided **as‑is** for personal and research use.

Redistribution is permitted provided this guide and author credit remain intact.

---

*Thank you for using GeoImage KMZ.*
