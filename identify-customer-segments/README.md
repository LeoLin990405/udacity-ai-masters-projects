# Identify Customer Segments

Unsupervised Learning Project — Udacity ML Nanodegree (Introduction to Machine Learning with PyTorch)

## Overview

Use unsupervised learning (PCA + K-Means) to identify demographic segments of the German population that form the core customer base for a mail-order sales company. Data provided by Bertelsmann Arvato Analytics.

## Pipeline

1. **Preprocessing**: Missing value encoding, column/row filtering, categorical re-encoding, mixed feature engineering
2. **Feature Transformation**: Median imputation → StandardScaler → PCA (80% variance retained)
3. **Clustering**: K-Means (k=10) on PCA-transformed data
4. **Comparison**: Customer vs general population cluster distributions

## Key Finding

The company's core customers are **older, financially conservative, family-oriented individuals in less urban West German areas**.

## Files

- `Identify_Customer_Segments.ipynb` — Main analysis notebook
- `report.html` — HTML export for submission
- `*.png` — Visualizations

## Data (not included)

Data files are proprietary (Arvato/Bertelsmann) and excluded per terms of use.

## Requirements

- Python 3, NumPy, pandas, scikit-learn, matplotlib, seaborn
