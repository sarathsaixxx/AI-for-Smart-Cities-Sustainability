# Delhi-NCR Land Cover Pipeline
*By D. Sarath Sai*

## Description
This pipeline performs the following tasks:

1. Loads Delhi-NCR and Delhi-Airshed boundaries from GeoJSON files.
2. Loads the WorldCover 2021 land-cover raster.
3. Ensures all layers share the same Coordinate Reference System (CRS).
4. Clips the raster to the Delhi-NCR region.
5. Plots the results, showing land-cover classes overlaid with Delhi-NCR (red) and airshed (blue) boundaries.

The resulting map provides a visual overview before further image filtering or analysis.

## Libraries Used

- **NumPy** – Fast numerical computations with arrays.
- **Xarray** – Adds labels to multi-dimensional arrays.
- **rioxarray** – Extends Xarray for geospatial raster operations.
- **GeoPandas** – Handles GeoJSON and spatial vector data.
- **Rasterio** – Raster I/O and spatial analysis.
- **Matplotlib / Seaborn** – Visualization.

> To install `rioxarray` in Colab:
```bash
!pip install rioxarray
