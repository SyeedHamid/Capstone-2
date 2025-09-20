# Climate Anomaly Prediction & Analysis

## Overview
This project uses historical climate datasets and machine learning to predict global temperature anomalies and assess model performance over time.  
It integrates Berkeley Earth and HadCRUT5 data, engineers lagged and rolling features, and benchmarks multiple models — including HistGradientBoosting, Random Forest, XGBoost, and a Residual Boosted hybrid — to identify the most accurate and stable predictor.

## Key Features
- **Data Integration**: Combines Berkeley Earth and HadCRUT5 datasets into a unified annual anomaly record.
- **Feature Engineering**: Decade grouping, lag features, rolling statistics, smoothed lags, and normalization.
- **Model Benchmarking**: Hyperparameter tuning with GridSearchCV; evaluation of four model architectures.
- **Performance Analysis**: Decade‑wise accuracy trends, residual bias detection, and ensemble averaging.
- **Recent Trends**: Threshold tracking (2016–2025) shows a slight shift toward moderate anomalies while high anomalies remain stable.

## Results
- **Best Model**: XGBoost (~99.96% accuracy in the 2020s).
- **Stability**: Residuals remain small across decades; early‑period divergence linked to sparse historical data.
- **Trend Insight**: Low anomalies decreased slightly, moderate anomalies increased, high anomalies steady.


## Author
Syeed — IT Analyst & Technical Support Specialist with expertise in climate data analysis, automation, and workflow optimisation

## License
This project is licensed under the MIT License — see the LICENSE file for details.

## Installation
```bash
git clone <your-repo-url>
cd <your-repo-folder>
pip install -r requirements.txt

**Usage**
jupyter notebook "Capstone 2.ipynb"

**Requirements**
Core packages:
pandas
numpy
xarray
netCDF4
scikit-learn
xgboost
matplotlib
seaborn

