# PaDayon eMap basemap

`misor-d2.zip` is the basemap for the PaDayon Pilipino eMap. It is a PMTiles file (not a zip archive): an OpenMapTiles vector tileset with a Northern Mindanao overview (zoom 0 to 10) and street-level detail for the 2nd District of Misamis Oriental (zoom 11 to 14).

- It is named `.zip` so that GitHub Pages serves it uncompressed. Pages compresses unknown binary types, and byte ranges over a compressed copy break PMTiles.
- It is served from GitHub Pages because Firebase Hosting does not serve correct byte ranges for it.
- The source and the build script are in the cbe-project-tracker repository (`scripts/build-district-map.sh`).

Map data © OpenStreetMap contributors (ODbL), built with Planetiler in the OpenMapTiles schema.
