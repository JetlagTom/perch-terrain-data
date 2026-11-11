# Perch Terrain Data

Elevation data assets (DTM/DSM GeoTIFFs) for a small personal project, hosted here as GitHub Release attachments so the main application repo can stay private.

Source: Land Steiermark, Airborne Laserscanning, CC BY 4.0.

## dem/v1/dem-alps-100m.bin

The terrain the Perch app reads on the phone for the whole Alpine region, a
tile at a time over HTTP range requests (it is served from
raw.githubusercontent.com, which allows both range requests and cross-origin
reads). 100m surface model in UTM 33N, 256x256 raw-deflate tiles with an
index - the format is documented in Perch's `data/scripts/build_offline_bundle.py`.
Files are never replaced in place; a rebuilt model goes under a new `vN/`.

Sources and attribution:

- Austria: Bundesamt für Eich- und Vermessungswesen (BEV) – data.bev.gv.at, ALS DSM, CC BY 4.0
- Everywhere else: Copernicus DEM GLO-30 – produced using Copernicus WorldDEM-30
  © DLR e.V. 2010-2014 and © Airbus Defence and Space GmbH 2014-2018, provided
  under COPERNICUS by the European Union and ESA; all rights reserved.
