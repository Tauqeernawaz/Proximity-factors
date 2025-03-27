# Proximity Factors Analysis: Distance from Settlements, Road Density, Built-up Areas, and Water Bodies

This repository contains the analysis of **proximity factors** including **distance from settlements (DS)**, **road network density (RND)**, **distance from built-up areas (DFBU)**, and **distance from water bodies (DFW)**. These factors were calculated using **Euclidean distance functions** in **GIS environments** and analyzed through **Kernel Density Estimation** in **ArcGIS 10.4.8**.

## Data Sources:
The following data were used for calculating the proximity factors:
- **OpenStreetMap (OSM)**: [https://www.openstreetmap.org/](https://www.openstreetmap.org/)
- **Built-up Areas**: Derived from satellite imagery (e.g., MODIS, Landsat).
- **Road Network**: Extracted from OSM for the study area.
- **Water Bodies**: Derived from available geospatial datasets (e.g., water body shapefiles).

## Methodology:
### 1. **Distance from Settlements (DS)**
   - Calculated using **Euclidean distance** functions in **ArcGIS**.
   - The **settlements layer** was extracted from **OpenStreetMap (OSM)** and processed to calculate the distance to the nearest settlement.

### 2. **Road Network Density (RND)**
   - The **road network density** was calculated using **Kernel Density Estimation**.
   - **Road network data** from **OSM** were used to create a density surface, representing the concentration of roads in the study area.

### 3. **Distance from Built-up Areas (DFBU)**
   - **Built-up areas** were identified using **satellite imagery** (MODIS or Landsat) and the distance to these areas was calculated using **Euclidean distance** functions.
   - **Buffer zones** around built-up areas were analyzed to assess the extent of urban sprawl.

### 4. **Distance from Water Bodies (DFW)**
   - **Water bodies** were extracted from relevant geospatial datasets (e.g., **shapefiles** of rivers, lakes, and wetlands).
   - **Euclidean distance** was used to calculate proximity to water bodies.

### 5. **GIS Tools Used:**
   - **ArcGIS 10.4.8**: For proximity analysis and kernel density estimation.
   - **QGIS** (optional): For visualizing the processed layers.
   
### 6. **Scripts and Functions Used:**
   - **ArcGIS Python Scripting**: Custom scripts were used to calculate distances and density.
   - **Kernel Density Estimation**: For analyzing road network density and built-up area patterns.

## How to Use:
1. **Download the Data**: Get the relevant shapefiles from **OpenStreetMap (OSM)** for settlements, roads, and water bodies. Built-up area data can be derived from **MODIS** or **Landsat** images.
2. **Run the Scripts**: Use the provided **ArcGIS** scripts or functions in **Python** to calculate the proximity factors:
   - **Distance from Settlements (DS)**
   - **Road Network Density (RND)**
   - **Distance from Built-up Areas (DFBU)**
   - **Distance from Water Bodies (DFW)**
3. Visualize the outputs in **ArcGIS** or **QGIS**.

## Citation:
If you use this methodology or data in your research, please cite the following:
