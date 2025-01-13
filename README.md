# GeoPandas-Mastery A-to-Z

## **Project 1: Geospatial Data Processing and Visualization**

### **Description**
This project focuses on processing and visualizing geospatial data using GeoPandas and Matplotlib. The operations performed include:

- **Shapefile Import and Plotting:** Imported and visualized district boundaries, areas of interest, and ATM locations.
- **Layer Reprojection:** Reprojected GeoDataFrames into a consistent coordinate reference system (EPSG:32629) for analysis.
- **Spatial Intersection:** Performed intersection between district boundaries and the area of interest to identify overlapping regions.
- **Area Calculation:** Computed the area of intersected regions and added it as a new attribute to the GeoDataFrame.
- **Shapefile Export:** Exported the processed GeoDataFrame to an ESRI Shapefile for further use.

### **Key Outcomes**
- Created detailed visualizations of geospatial layers.
- Derived geospatial insights such as intersected areas.
- Prepared datasets for future analysis by exporting the processed layers.

---
## **Project 2: Global Land Area Analysis**

### **Description**
This project involved analyzing and visualizing global land areas using GeoPandas. The key operations include:

- **Shapefile Import and Area Calculation:** Imported a world shapefile, calculated the area of each country, and removed Antarctica from the dataset.
- **Projection Transformation:** Changed the coordinate reference system to EPSG:3857 for better visualization and re-calculated areas in square kilometers.
- **Visual Enhancements:**
  - Plotted world regions with a color-coded scheme (`hsv`).
  - Added a legend displaying the area of countries in square kilometers.
  - Resized and repositioned the legend for clarity.

### **Key Outcomes**
- Gained insights into the geographical distribution and size of countries.
- Created visually appealing global maps with detailed legends for enhanced understanding.
- Refined projection techniques for accurate spatial analysis.

---

## **Project 3: Global Airport Mapping**

### **Description**
This project focuses on mapping global airport locations and creating geospatial datasets. The operations performed include:

- **CSV to GeoDataFrame Conversion:** Read a CSV file containing airport data and converted it into a GeoPandas GeoDataFrame using longitude and latitude values.
- **Data Visualization:** Plotted airport locations on a map, customizing marker sizes and map dimensions for clarity.
- **Projection Definition:** Defined the spatial reference system using the ESRI Well-Known Text (WKT) format to ensure consistent geographic representation.
- **Shapefile Export:** Saved the GeoDataFrame as an ESRI Shapefile for use in GIS applications.

### **Key Outcomes**
- Mapped global airport locations effectively using GeoPandas.
- Ensured compatibility with GIS tools by exporting datasets with a defined spatial reference system.
- Enhanced understanding of geospatial operations related to point data.

---
## **Project 4: Topographic Elevation Extraction**

### **Description**
This project demonstrates the extraction of topographic elevation data from a DEM (Digital Elevation Model) to point features. The key operations include:

- **Shapefile Import:** Read a shapefile containing station locations.
- **Elevation Extraction:**
  - Iteratively extracted elevation values for each station point by matching its coordinates with the corresponding pixel in the DEM.
  - Used Rasterio for efficient raster data handling.
- **Data Enrichment:** Added the extracted elevation values as a new attribute to the GeoDataFrame.
- **CSV Export:** Saved the enriched data, including station names and elevations, into a CSV file for further analysis.

### **Key Outcomes**
- Successfully integrated raster and vector data for geospatial analysis.
- Generated elevation data for specific locations, facilitating further topographic studies.
- Created a reusable process for extracting raster-based attributes to vector layers.
