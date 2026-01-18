# Indian-Monsoon-Precipitation-Analysis
## 🛠️ Technical Implementation
* **Data Engineering:** Utilized `xarray` to manipulate multi-dimensional NetCDF climate data (ERA5 Reanalysis).
* **Dimensionality Reduction:** Handled the "Curse of Dimensionality" (135k+ features vs 60 samples) using correlation mapping for feature selection.
* **Math from Scratch:** Implemented **Linear Ridge Regression** using the Normal Equation via `numpy.linalg`, rather than relying on high-level Scikit-Learn abstractions.
* **Regularization:** Tuned L2 Penalty to resolve LinAlg errors and prevent overfitting on stochastic climate data.
