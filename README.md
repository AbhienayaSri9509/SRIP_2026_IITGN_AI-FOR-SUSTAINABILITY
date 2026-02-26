🌍 Land Use & Spatial Analysis of Delhi NCR using ESA WorldCover 2021
📌 Project Overview

This project performs geospatial analysis of Delhi NCR using:

ESA WorldCover 2021 Land Use/Land Cover raster data

Delhi NCR administrative boundary

Delhi Airshed boundary

The objective is to:

Clip land cover raster to NCR boundary

Align coordinate systems (CRS)

Visualize spatial distribution

Enable further land-use classification and environmental analysis

📂 Dataset Description
1️⃣ ESA WorldCover 2021

File: worldcover_bbox_delhi_ncr_2021.tif

Resolution: 10m

Format: GeoTIFF

Contains land cover classes such as:

Built-up

Cropland

Trees

Grassland

Water

Shrubland

Bare land

Source: European Space Agency (ESA)

2️⃣ Delhi NCR Region Boundary

File: delhi_ncr_region.geojson

Format: GeoJSON

Defines administrative boundary of Delhi NCR

3️⃣ Delhi Airshed Boundary

File: delhi_airshed.geojson

Format: GeoJSON

Represents atmospheric influence boundary used for air quality analysis

🛠️ Technologies Used

Python 3

Google Colab

GeoPandas

Rasterio

Rioxarray

Matplotlib

Shapely

⚙️ Methodology
Step 1: Load Vector Data

Read NCR and Airshed GeoJSON files using GeoPandas.

Step 2: Load Raster Data

Open ESA WorldCover GeoTIFF using rioxarray.

Step 3: Coordinate Reference System (CRS) Alignment

Convert vector boundaries to match raster CRS.

Step 4: Raster Clipping

Clip raster to NCR boundary.

Step 5: Visualization

Plot clipped raster.

Overlay NCR and Airshed boundaries.

📊 Output

The output includes:

Clipped WorldCover raster for Delhi NCR

Visual map showing:

Land cover distribution

NCR boundary

Airshed boundary

📌 Applications

This analysis can be extended for:

Built-up area estimation

Green cover percentage calculation

Urban expansion monitoring

Environmental impact assessment

Air quality modeling support

Sustainable urban planning research

🚀 How to Run

Upload the following files to Google Colab:

worldcover_bbox_delhi_ncr_2021.tif

delhi_ncr_region.geojson

delhi_airshed.geojson

Install required libraries:

pip install geopandas rasterio rioxarray shapely matplotlib

Run the Python script provided in the notebook.

📈 Future Improvements

Land cover class area calculation

Zonal statistics

Grid-based spatial analysis

Time-series comparison (multi-year data)

Integration with air pollution datasets

👩‍💻 Author

Abhienaya Sri
Final Year Student
Geospatial & AI Research Enthusiast
