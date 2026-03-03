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

# How to Run the Project (If You Want to Run It Using Open-Source Tools Like VS Code, etc.)

## 1. Clone the Repository

```bash
git clone <your-repo-link>
cd <your-repo-folder>
```

## 2. Create Virtual Environment (Recommended)

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## 4. Setup Kaggle API

1. Go to Kaggle → Account → Create New API Token
2. Download `kaggle.json`
3. Place it in:

* **Windows:** `C:\Users\<your-username>\.kaggle\`
* **Mac/Linux:** `~/.kaggle/`

(Mac/Linux only)

```bash
chmod 600 ~/.kaggle/kaggle.json
```

## 5. Open the Notebook

Open the `.ipynb` file in VS Code (or Jupyter Notebook) and run all cells.

---

The dataset will download automatically, and the models (TinyCNN and ResNet18) will train and evaluate.

