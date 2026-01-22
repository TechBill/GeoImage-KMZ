# GeoImage KMZ – User Guide

---

## Overview

GeoImage KMZ is a lightweight, standalone desktop application designed for historical and exploratory map research. It helps you align scanned or photographed maps (plat maps, railroad maps, atlases, aerials, etc.) with modern geographic coordinates so they can be overlaid in Google Earth and other KMZ-compatible tools.

The app is intentionally simple and fast, focusing on research and field scouting rather than survey-grade GIS accuracy.

---

## Paste Coordinates Feature

GeoImage KMZ includes a **Paste Coordinates** button in the *Enter Coordinates* dialog to speed up adding control points.

Instead of typing latitude and longitude manually, you can copy coordinates from common mapping tools and paste them directly. The app automatically extracts and fills the Latitude and Longitude fields.

---

### Google Earth Pro

Google Earth Pro does not support direct right-click copying of map coordinates. Instead, use a placemark:

1. Click **Add Placemark** (yellow pushpin icon)
2. Move the placemark to the desired location
3. Click **OK** to close the placemark information window
4. Right-click directly on the **placemark pin on the map**
5. Choose **Copy**
6. Click **Paste Coordinates** in GeoImage KMZ

GeoImage KMZ automatically extracts the latitude and longitude from the copied KML.

---

### Google Maps

1. Right-click anywhere on the map
2. Click the coordinates shown in the menu
3. The coordinates are copied to the clipboard
4. Click **Paste Coordinates** in GeoImage KMZ

Example:
```
38.627003, -90.199402
```

---

### QGIS

1. Load a basemap (e.g., OpenStreetMap) in QGIS
2. Right-click anywhere on the map → **Copy Coordinate**
3. Select **EPSG:4326 – WGS 84**
4. Click **Paste Coordinates** in GeoImage KMZ

⚠️ Do not use projected coordinate systems such as **EPSG:3857** (meters).

---

### Supported Paste Formats

GeoImage KMZ supports common formats including:

- `38.627003, -90.199402`
- `38.627003 -90.199402`
- `-90.199402,38.627003,0` (Google Earth KML)
- Text containing valid latitude and longitude values

---

## Rotation Reminder

- Rotating the image clears all control points
- Always rotate **before** adding points

---

## Troubleshooting Notes

If pasted coordinates do not appear:
- Ensure the values are latitude/longitude in decimal degrees
- Avoid meter-based projected coordinates
- Try copying again from the source tool

---

## License & Credits

GeoImage KMZ is provided **as-is** for personal and research use.

Redistribution is permitted provided this guide and author credit remain intact.

---

## Support & Contact

GeoImage KMZ is a free tool created for historical researchers, genealogists, and metal detecting enthusiasts.

If you find it useful, please consider supporting development:

- PayPal: https://www.paypal.com/paypalme/techbill
- Buy Me a Coffee: https://buymeacoffee.com/techbill

**Author:** Bill Fleming (TechBill)
**GitHub:** https://github.com/TechBill

---

*Thank you for using GeoImage KMZ.*
