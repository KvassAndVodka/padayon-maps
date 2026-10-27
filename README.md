# PaDayon eMap basemap

`misor-d2.zip` is the basemap for the PaDayon Pilipino eMap. It is a PMTiles file (not a zip archive): an OpenMapTiles vector tileset with a Northern Mindanao overview (zoom 0 to 10) and street-level detail for the 2nd District of Misamis Oriental (zoom 11 to 14).

`misor-dem.zip` is the 3D terrain for the same eMap. It is also a PMTiles file: Copernicus GLO-30 elevation for the Northern Mindanao overview area, as Terrarium-encoded WebP tiles (zoom 0 to 12).

Both files follow these rules:

- Each is named `.zip` so that GitHub Pages serves it uncompressed. Pages compresses unknown binary types, and byte ranges over a compressed copy break PMTiles.
- They are served from GitHub Pages because Firebase Hosting does not serve correct byte ranges for them.
- The source and the build scripts are in the cbe-project-tracker repository (`scripts/build-district-map.sh` and `scripts/build-terrain-map.py`).

Map data © OpenStreetMap contributors (ODbL), built with Planetiler in the OpenMapTiles schema.

Elevation: produced using Copernicus WorldDEM-30 © DLR e.V. 2010-2014 and © Airbus 2014-2018, provided under COPERNICUS by the European Union and ESA.
