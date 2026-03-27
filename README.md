# Watershed Delineation using QGIS

## Overview
This project demonstrates watershed delineation using a Digital Elevation Model (DEM) in QGIS. The workflow includes DEM preprocessing, stream network extraction, and watershed boundary generation for a defined outlet point.

## Objectives
- Delineate watershed from DEM data  
- Extract stream network using flow accumulation  
- Generate a final map layout with proper cartographic elements  

## Data Used
- **DEM Source**: ISRO Bhuvan  
- **Coordinate System**: WGS 84 / UTM Zone 43N (EPSG:32643)

## Tools & Software
- QGIS 3.16  
- QGIS Processing Toolbox

## GIS Tools Used
The following QGIS Processing Toolbox tools were used in this project:
- **Fill Sinks (Wang & Liu)**  
  Used to remove depressions in the DEM to ensure proper flow direction.
- **Strahler Order**  
  Used to classify stream hierarchy and determine stream order.
- **Channel Network and Drainage Basins**  
  Used to extract stream networks based on flow accumulation threshold.
- **Upslope Area**  
  Used to delineate watershed boundary based on a defined outlet point.
- **Polygon Clipping (Clip Vector)**  
  Used to clip stream network within the watershed boundary.
- **Clip Raster by Mask Layer**  
  Used to clip DEM data to the watershed area.

## Methodology
1. Load DEM and reproject to UTM  
2. Fill sinks in DEM (Wang & Liu method)  
3. Generate flow direction and flow accumulation  
4. Extract stream network using threshold value  
5. Define outlet point  
6. Generate watershed using upslope area method  
7. Convert raster to vector  
8. Clip streams and DEM to watershed boundary  
9. Create final map layout  

## Outputs
- Watershed boundary (vector)  
- Stream network (vector)  
- Clipped DEM (raster)  
- Final map layout  

## Skills Demonstrated
- Raster analysis  
- Hydrological modeling  
- GIS data processing  
- Map layout design  

## Results
The final output includes a watershed boundary with extracted stream network overlaid on a DEM background, presented with legend, scale bar, and north arrow.

## Future Improvements
- Integrate rainfall and land use data  
- Perform runoff analysis  
- Automate workflow using Python (PyQGIS)  

## Author
Arun Krishnan K
