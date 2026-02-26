# 🌍 Spatial Analysis of Land Use in Delhi NCR Using ESA WorldCover 2021
## 1. Project Overview

This project performs geospatial analysis of land use and land cover (LULC) patterns in the Delhi National Capital Region (NCR) using high-resolution ESA WorldCover 2021 data.

The primary objective is to integrate raster-based land cover data with administrative and environmental boundary datasets to support urban and environmental analysis.

The workflow includes raster clipping, coordinate system harmonization, and spatial visualization of land cover distribution within Delhi NCR and its associated airshed region.

## 2. Study Area

The study focuses on:

Delhi NCR Administrative Boundary

Delhi Airshed Boundary

These regions are used to spatially constrain and contextualize land cover analysis.

## 3. Datasets Used
3.1 ESA WorldCover 2021

File: worldcover_bbox_delhi_ncr_2021.tif

Type: Raster (GeoTIFF)

Resolution: 10 meters

Source: European Space Agency (ESA)

Description: Global land cover dataset containing classified land use categories such as built-up areas, cropland, trees, grassland, water bodies, shrubland, and bare land.

3.2 Delhi NCR Boundary

File: delhi_ncr_region.geojson

Format: GeoJSON

Description: Administrative boundary defining the spatial extent of Delhi NCR.

3.3 Delhi Airshed Boundary

File: delhi_airshed.geojson

Format: GeoJSON

Description: Environmental boundary representing atmospheric influence zone relevant for air quality and pollution modeling studies.

## 4. Methodology

The analysis pipeline consists of the following steps:

Step 1: Data Ingestion

Vector datasets are loaded using GeoPandas.

Raster dataset is loaded using rioxarray.

Step 2: Coordinate Reference System (CRS) Alignment

All vector layers are reprojected to match the raster CRS to ensure spatial consistency.

Step 3: Raster Clipping

The WorldCover raster is clipped to the Delhi NCR boundary.

This reduces computational load and restricts analysis to the study region.

Step 4: Spatial Visualization

Clipped raster is visualized.

NCR and Airshed boundaries are overlaid for spatial interpretation.

## 5. Tools and Technologies

Python 3.x

Google Colab

GeoPandas

Rasterio

Rioxarray

Shapely

Matplotlib

## 6. Output

The output of this project includes:

Clipped land cover raster specific to Delhi NCR.

Integrated visualization of:

Land cover distribution

NCR boundary

Airshed boundary

These outputs form the foundation for further quantitative spatial analysis.

## 7. Potential Extensions

This framework can be extended to:

Built-up area quantification

Green cover percentage analysis

Zonal statistics computation

Grid-based urban expansion modeling

Integration with air pollution or meteorological datasets

Multi-temporal land cover change detection

## 8. Reproducibility

To reproduce this analysis:

Upload the following files:

worldcover_bbox_delhi_ncr_2021.tif

delhi_ncr_region.geojson

delhi_airshed.geojson

Install required libraries:

pip install geopandas rasterio rioxarray shapely matplotlib

Execute the provided Python script in a Jupyter/Colab environment.

## 9. Author

Abhienaya Sri

Final Year Student

Geospatial Data Analysis & AI Research
