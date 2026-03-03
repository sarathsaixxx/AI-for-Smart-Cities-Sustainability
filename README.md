[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E81TFsdBh_hlXzM3eZcxNqAwZT5JKqld?usp=sharing)
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
```

And refer this readme Documentation:  [README.pdf](https://github.com/sarathsaixxx/AI-for-Smart-Cities/blob/main/readme_documentation.pdf)

### OR

Refer to this drive link (if the above link crashes):  [README.pdf](https://drive.google.com/file/d/1OfBO1ERXs-fNfbAqFkUEK0qB-ZcoA-hI/view?usp=sharing)
