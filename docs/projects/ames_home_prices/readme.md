B"H

[← Back to Home](/)

# Predicting Home Sale Prices and Discovering Correlations in Ames, Iowa

## Research Question
How accurately can we predict a home's sale price using routine listing and property characteristics, and which features most strongly drive residential property values in Ames, Iowa?

## Project Overview
This project builds transparent and performant models to predict home sale prices from property characteristics using the widely-used Ames Housing dataset, which contains 1,460 property sales with 79 explanatory variables spanning the 2006-2010 period in Ames, Iowa. The goal is to provide accurate price estimation for real-estate professionals, appraisers, and homeowners while clearly communicating which features most strongly drive price.

The analysis encompasses three major components:

1. **Data Exploration & Preparation** - Handling high-missing columns (PoolQC 99.5%, MiscFeature 96%, Alley 93.8%, Fence 80.8%), treating "NA" values that encode true absence vs. missingness, applying log transformation to right-skewed SalePrice target, and preparing mixed-type features (lot/neighborhood descriptors, structure quality/size, basement/garage details, kitchen/bath conditions)

2. **Model Development & Comparison** - Training baseline models including Ridge regression, Random Forest, and Gradient Boosting (XGBoost/LightGBM) with 5-fold cross-validation, using median/mode imputation, scaling, and one-hot encoding, with early stopping and hyperparameter tuning to optimize RMSE, MAE, and R² metrics

3. **Interpretation & Feature Analysis** - Extracting standardized coefficients from linear models, permutation importance and SHAP values from tree-based models, partial dependence plots, and correlation heatmaps to identify dominant price drivers (OverallQual, GrLivArea, TotalBsmtSF, garage capacity) and communicate stakeholder-friendly explanations

The project demonstrates comprehensive regression modeling practices including proper handling of mixed data types, missing value semantics, transformation strategies for skewed targets, and model-agnostic interpretability techniques. Final results show Gradient Boosting achieving the strongest performance (RMSE ≈ 28.4K, R² ≈ 0.851), with size and overall quality confirmed as dominant price drivers through both correlation structure and tree-based importance analysis.

## Project Files
- [Jupyter Notebook](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/ames_home_prices/notebook.ipynb)
- [White Paper (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/ames_home_prices/white_paper.pdf)

