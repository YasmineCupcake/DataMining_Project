# DATA MINING – Practical Work Project  
**Forest Fire Prediction and Risk Analysis**

## Overview
Forest fires represent a major environmental and socio-economic challenge, causing
vegetation loss, soil degradation, and severe ecological damage.  
Early prediction of fire occurrence is essential for effective prevention and management.

This project develops a **data-driven predictive system** using **soil characteristics** and
**climate variables** to forecast forest fire occurrence and identify high-risk zones.
Both **supervised** and **unsupervised** machine learning techniques are applied, with
implementations developed **from scratch** and compared with Scikit-learn models.

## Study Area
- **Countries**: Algeria & Tunisia (grouped in the same dataset)
- **Year**: 2024
- **Academic Context**:  
  Students: ALLAF Chaima + Boutkedjirt Aya
  USTHB – Faculty of Computer Science  
  IASD – M2 SII  
  Academic Year: 2025/2026

---

## Project Objectives
- Collect and preprocess soil and climate data relevant to fire prediction
- Predict fire occurrence using supervised learning algorithms
- Identify natural clusters and high-risk fire areas using unsupervised learning
- Evaluate models using standard performance metrics
- Provide interpretable insights for fire risk analysis

---

## Data Mining Methodology

### Step 1: Data Analysis and Preprocessing
- Exploratory Data Analysis (EDA)
- Data cleaning and preprocessing
- Data integration (soil, climate, fire, elevation)
- Feature engineering

### Step 2: Supervised Machine Learning
Algorithms implemented **from scratch**:
- K-Nearest Neighbors (KNN)
- Decision Trees
- Random Forest

Evaluation:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

Comparative analysis with **Scikit-learn implementations**.

### Step 3: Unsupervised Machine Learning (Clustering)
Algorithms implemented **from scratch**:
- K-Means
- DBSCAN
- CLARANS

Evaluation and comparison with Scikit-learn clustering algorithms.

---

## Datasets

### Fire Dataset
Source: NASA FIRMS (VIIRS NOAA-20, 2024)
- Algeria: https://firms.modaps.eosdis.nasa.gov/country/
- Tunisia: https://firms.modaps.eosdis.nasa.gov/country/

### Land Cover Dataset
- Algeria: FAO Land Cover  
- Tunisia: FAO Land Cover

### Climate Dataset
- WorldClim Monthly Weather Data (5-minute resolution)  
  https://worldclim.org/data/monthlywth.html

### Elevation Dataset
- GMTED2010  
  https://edcintl.cr.usgs.gov/downloads/sciweb1/shared/topo/downloads/GMTED/Grid_ZipFiles/be15_grd.zip

### Soil Dataset
- Harmonized World Soil Database v2.0 (FAO)

Extracted from table **HWSD2_LAYERS**:
- Only **LAYER = D1** (first 20 cm soil depth)

Selected features:
COARSE, SAND, SILT, CLAY, TEXTURE_USDA, TEXTURE_SOTER, BULK, REF_BULK,
ORG_CARBON, PH_WATER, TOTAL_N, CN_RATIO, CEC_SOIL, CEC_CLAY, CEC_EFF,
TEB, BSAT, ALUM_SAT, ESP, TCARBON_EQ, GYPSUM, ELEC_COND

---

## Project Structure
Jupyter notebooks (analysis, models, evaluation)

---

## How to Run the Project
1. Install the libraries that are mentioned in the notebooks
2. Install the datasets
3. Run notebooks in the provided order(without loading)


---

## Notes
- Raw datasets are not included due to size limitations.
- All machine learning algorithms are implemented **from scratch** + sklearn.
- Results are reproducible using the provided code and methodology.
- Clarans didn't run properly because the sklearn.extra + numpy libraries needed python 10 so execute with caution (it's preferable to execute it on colab or any external method or environment)



[Download datasets](https://drive.google.com/drive/folders/xxxxxxxxxxxx)
