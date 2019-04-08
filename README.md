#BCN ENERGY provides codes for reading KML files and reconstructing architectural geometries.

The purpose of this project is to analyze the solar radiation, daylight, daylit and energy consumption of the buildings of Barcelona. This section focuses exclusively on the localization and construction of the geometry, while the analysis is run in Rhino Grasshopper, with LadyBug and HoneyBee.

The KML files are divided into high-detailed geometries (buildings to analyze) and low-detailed geometries (context buildings).
KMLs L files include the geodetic coordinates of the base points of the geometry and the height of the building (construction of the base + extrusion).
KMLs H files are divided per building local, each local includes the geodetic coordinates of each surface. The geometry constructed is therefore divided per floors, each floor is divided per local. Further details, such as local use and name, are specified in this type of file.

The transformation of geodetic coordinates to carthesian coordinates is done with the use of pyproj EPSG 25831.
