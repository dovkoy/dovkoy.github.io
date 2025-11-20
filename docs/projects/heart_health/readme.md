B"H

[← Back to Home](/)

# Heart Disease Risk Prediction: Interpretable Clinical Decision Support

## Research Question
Can we accurately predict the presence of heart disease using routinely collected clinical attributes, and which factors most strongly influence cardiovascular risk to support preventative care and early intervention?

## Project Overview
This project develops an interpretable, end-to-end analysis for predicting the presence of heart disease using the well-studied UCI Heart Disease dataset (Cleveland subset). The goal is to create a concise, ethical, and actionable modeling workflow that identifies key risk factors and supports practical decision-making for health systems and clinicians, demonstrating a proof of concept for preventative care and early intervention tools.

The analysis encompasses three major components:

1. **Data Preparation & Exploration** - Working with 304 records from the Cleveland cohort, defining binary target (presence of disease when angiographic label > 0), handling mixed data types (demographics, clinical measures), performing stratified train/test split (25% held out), and conducting EDA to examine class balance, age distributions, and chest pain presentation patterns

2. **Model Development & Evaluation** - Training two models: Logistic Regression as a transparent baseline and Random Forest as a non-linear benchmark, both using class-balanced weighting, preprocessing pipelines with median imputation for numeric features and one-hot encoding for categoricals, and comprehensive evaluation using accuracy, precision, recall, F1, ROC-AUC, confusion matrices, and 5-fold stratified cross-validation

3. **Interpretation & Clinical Insights** - Extracting odds ratios from Logistic Regression highlighting risk-increasing associations (vessel count, asymptomatic chest pain, reversible thal defects) and protective associations (female sex, typical angina, higher maximum heart rate), complemented by Random Forest permutation importances emphasizing ECG and chest-pain markers

The project demonstrates rigorous clinical modeling practices including proper handling of missingness without leakage, class imbalance management, interpretability prioritization, and ethical considerations for healthcare applications. Both models achieve strong discrimination (Logistic Regression: ROC-AUC 0.936, Random Forest: ROC-AUC 0.952 on single split; RF cross-validation: ROC-AUC ≈ 0.915), with the logistic model providing transparent, clinically sensible risk drivers suitable for point-of-care decision support.

## Project Files
- [Jupyter Notebook](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/heart_health/notebook.ipynb)
- [White Paper (PDF)](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/heart_health/white_paper.pdf)

