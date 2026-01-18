# Indian Monsoon Precipitation Analysis

## 🌏 Project Overview
A comprehensive climate data analysis repository focused on modeling and predicting Indian Summer Monsoon Rainfall (ISMR) patterns. Developed as part of the M.Tech curriculum in Climate Change at IIT Hyderabad, this project applies Machine Learning and Statistical methods to raw satellite/station data (NetCDF).

## 🔬 Research Modules
This repository contains multiple analysis modules ranging from raw data processing to advanced dimensionality reduction.

### 1. Core Implementation: Ridge Regression from Scratch
* **File:** `cda monsoon project (1).ipynb`
* **Objective:** Predict seasonal rainfall using Winter Sea Surface Temperatures (SST).
* **Methodology:** Implemented **Linear Ridge Regression** using the Normal Equation via `numpy.linalg` (no high-level abstractions).
* **Key Tech:** Solved the "Curse of Dimensionality" (135k+ features vs 60 samples) using correlation mapping.

### 2. Spatio-Temporal Pattern Recognition
* **File:** `1_SST_EOF_Analysis.ipynb`
* **Objective:** Identify dominant climate drivers (like El Niño).
* **Methodology:** Performed **Empirical Orthogonal Function (EOF)** analysis on Sea Surface Temperature anomalies to extract Principal Components.

### 3. Model Benchmarking
* **File:** `2_Model_Benchmarking_Ridge_Lasso.ipynb`
* **Objective:** Compare regression techniques for optimal forecasting.
* **Methodology:** Benchmarked **OLS vs. Ridge vs. Lasso** using `SequentialFeatureSelector`. Lasso achieved the lowest RMSE (1.44) on test data.

### 4. Long-Term Trend Analysis
* **File:** `3_CO2_Trend_Forecasting.ipynb`
* **Objective:** Analyze global atmospheric changes.
* **Methodology:** Time-series forecasting of CO2 concentrations using linear trend estimation.

## 💻 Tech Stack
* **Language:** Python 3.8+
* **Climate Data:** Xarray, NetCDF4 (ERA5 Reanalysis Data)
* **Computation:** NumPy (Linear Algebra), Pandas
* **Visualization:** Matplotlib, Cartopy, Seaborn

## 📊 Key Results
* **Dimensionality:** Successfully reduced 135,201 spatial features to relevant predictors without losing signal.
* **Stability:** Regularization (L2 Penalty) eliminated LinAlg singular matrix errors present in standard OLS.
* **Forecasting:** Detected strong inter-annual variability in Southern Peninsular India rainfall.

---
*Author: [Your Name] | M.Tech, Climate Change @ IIT Hyderabad*
