# Map 675
## Assignment 1: Mapping Atlanta
### Gaining command of GIS processing

This map was created using git and gdal/ogr commands in terminal. 

### Data clean up
Data sets include shapefiles for Atlanta city limits, transit routes, neighborhoods, and 2016 census. 

OGR was used to perform an inverse projection to the coordinate reference system NAD 83 and then transformed to WGS84 for web mapping. After that, we used `ogr2ogr -f` (flag) to change the file format to GeoJSON.

Mapshaper was used to simplify large files that were larger than 2mbs to improve map load time.

### Final notes
While working on assignment2 of this module, I realized I inadvertently removed the drawMap funtion from this map. It does not appear to have any impact as the layers are being drawn using ```L.GeoJSON {} addTo.map;```. I left this as is for the sake of simplicity but will watch for missing drawMap()s in the future.. Could be a fluke that everything still worked...

I left all of my working data files in the data folder for reference/to show my work for this project. 

