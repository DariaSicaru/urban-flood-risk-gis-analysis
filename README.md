
# Urban Flood Risk Assessment Using GIS – Bucharest, Romania

## Overview

This project focuses on the spatial assessment of potential flood risk in Bucharest, Romania, using Geographic Information Systems (GIS).

The study integrates topographic, hydrological and land use data to identify areas potentially susceptible to flooding based on selected natural and anthropogenic factors.

A GIS-based multi-criteria analysis was implemented in QGIS to evaluate the spatial distribution of flood risk across the municipality.

## Objectives

- Analyze the main physical and anthropogenic factors influencing urban flood risk.
- Identify areas potentially susceptible to water accumulation and flooding.
- Integrate multiple spatial datasets into a unified GIS-based assessment.
- Produce a flood risk map to support urban planning and risk management.

## Study Area

The study focuses on Bucharest, the capital of Romania, located in the Romanian Plain.

The city's relatively low relief, urban development, extensive impervious surfaces and hydrological network contribute to its potential vulnerability to urban flooding.

## Data and Methodology

The analysis was conducted in QGIS 3.40.4 using the following spatial datasets:

- **Digital Elevation Model (DEM):** GLO-30 Defence Gridded Elevation Data, ESA/PRISM, 30 m resolution.
- **Hydrography:** Rivers and lakes extracted from OpenStreetMap using QuickOSM.
- **Land Use and Land Cover:** CORINE Land Cover 2018.
- **Coordinate Reference System:** Stereo 70 (EPSG:3844).

Three main factors were integrated into the spatial assessment:

1. **Slope:** Lower slope values were assigned higher risk scores due to their potential to favor water accumulation.
2. **Distance to rivers:** Areas closer to watercourses were assigned higher risk scores.
3. **Land use and land cover (LULC):** Built-up and industrial areas received higher scores, while vegetated areas received lower scores.

Each factor was reclassified into five risk classes. The resulting rasters were combined using an equal-weight arithmetic mean through the QGIS Raster Calculator.

## Results

The final analysis produced a spatial flood risk map with five classes, ranging from very low to very high.

The results indicate:

- Medium-risk areas represent approximately 60% of the study area.
- High and very high risk areas are mainly associated with densely urbanized zones, low slopes and proximity to rivers and lakes.
- Lower-risk areas are more prevalent in parts of the western and southern outskirts.

## Limitations

The assessment represents a GIS-based spatial susceptibility/risk screening rather than a hydrodynamic flood simulation.

The main limitations include:

- Rainfall was not incorporated as a spatially variable raster factor.
- Equal weights were used due to the lack of locally validated weighting coefficients.
- Historical flood records were not available for model validation.
- The spatial resolution of the input datasets limits the level of local detail.


The project report and map legends are currently available in Romanian. The repository documentation may be updated with English versions in the future.

## Author

**Daria Sicaru**  
Applied Informatics in Environmental Engineering  
National University of Science and Technology POLITEHNICA Bucharest  
2026
