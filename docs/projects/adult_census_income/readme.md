B"H

[← Back to Home](/)

# Predicting Census Income Categories and Interpreting Socioeconomic Drivers

## Research Question
Can we accurately predict whether an individual's annual income exceeds $50,000 based on routine census metrics, and what are the key socioeconomic drivers that influence income classification?

## Project Overview
This project develops and evaluates interpretable machine learning models for classifying whether an adult's annual income exceeds $50,000 using the Adult Census Income dataset from the 1994 U.S. Census Bureau Current Population Survey. The objective is twofold: achieve reliable predictive performance on held-out data, and provide transparent explanations of the key drivers associated with higher income to inform workforce development agencies, policy makers, and employers.

The analysis encompasses three major components:

1. **Data Preparation & Exploration** - Standardizing schema, mapping literal "?" missing values to explicit "Unknown" categories, normalizing column names to snake_case, and creating a stratified 80/20 train/test split on 32,561 records with 16 features (numeric: age, hours_per_week, capital_gain, capital_loss; categorical: workclass, education, marital_status, occupation, relationship, sex, race, native_country)

2. **Model Development & Evaluation** - Training two baseline models inside leak-safe pipelines: Logistic Regression with L2 regularization and Random Forest with 200 trees, both using standardized numeric features and one-hot encoded categoricals, evaluated on held-out test data using accuracy, precision, recall, F1, and ROC-AUC metrics

3. **Interpretation & Subgroup Analysis** - Extracting and visualizing largest-magnitude Logistic Regression coefficients and top Random Forest feature importances to identify influential drivers, complemented by subgroup evaluation across sex and race to surface performance disparities and fairness considerations

The project demonstrates production-grade modeling practices including proper data leakage prevention, stratified sampling for class imbalance, comprehensive evaluation metrics, and transparent model interpretation. Key findings reveal capital gain, marital status, education, hours worked, and age as dominant income predictors, with both models achieving strong performance (ROC-AUC ≈ 0.90) and highlighting the need for calibrated thresholds and fairness-aware review before operational deployment.

## Project Files
- [Jupyter Notebook](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/adult_census_income/notebook.ipynb)
- [White Paper (PDF)](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/adult_census_income/white_paper.pdf)

