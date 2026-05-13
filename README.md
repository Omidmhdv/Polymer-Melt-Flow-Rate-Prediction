Polymer Melt Flow Rate Prediction
A regression case study for DS5006 predicting polymer Melt Flow Rate (MFR) from industrial reactor process variables using scikit-learn.
📋 Overview
Models a real-time "soft sensor" (digital twin) to predict MFR continuously between infrequent lab samples (~2–8 hrs apart).
📊 Dataset
Industrial reactor data with features: C3, H2R, Pressure, Level, C2, Cat, Temp → Target: MFR
🔧 Pipeline

Data loading & cleaning (missing values, outlier removal)
EDA — correlation heatmaps, pair plots, ydata-profiling
Feature selection (SelectKBest)
Data transformations (log, StandardScaler)
Regression modeling (Linear, Ridge, Lasso, KNN, Bayesian Ridge)
Bimodal distribution handling — split regression on lnMFR < 0 and lnMFR > 0

📦 Dependencies
pandas, numpy, scikit-learn, seaborn, matplotlib, plotly, ydata-profiling
📖 Reference
Hedengren, J.D. (2021) — APMonitor
