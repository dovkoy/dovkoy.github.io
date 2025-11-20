B"H

[← Back to Home](/)

# Customer Churn Prediction in Telecom Services

## Research Question
Can we accurately predict which telecom customers are likely to churn, and what are the primary drivers of customer retention that can inform targeted retention strategies?

## Project Overview
This project develops predictive models for customer churn in the telecommunications industry using the IBM Telco Customer Churn dataset containing information for approximately 7,000 customers. Customer churn directly impacts a telecom company's bottom line, with industry research indicating that acquiring a new customer costs 5-25 times more than retaining an existing one. The goal is to accurately predict which customers are likely to churn and identify key factors that contribute to retention.

The analysis encompasses three major components:

1. **Exploratory Data Analysis** - Examining 7,043 customer records with 21 features including demographics (gender, senior citizen status, partners, dependents), account information (tenure, contract type, payment method), services subscribed (phone, internet, tech support, online security), and billing information, identifying moderate class imbalance (26.5% churn rate) and key patterns such as contract type being the strongest predictor

2. **Data Preparation & Modeling** - Converting TotalCharges to numeric, binary-encoding the target variable, separating numeric and categorical features, building preprocessing pipelines with StandardScaler and OneHotEncoder, and training class-weighted Logistic Regression models with stratified 75/25 train/test split and 5-fold cross-validation

3. **Model Evaluation & Business Recommendations** - Achieving ROC-AUC of 0.846 on held-out test data with recall of 0.80 (capturing 8 out of 10 churners), interpreting model coefficients to identify key drivers (tenure, contract type, internet service type, payment method, monthly charges), and formulating actionable recommendations for retention campaigns

The project demonstrates production-grade customer analytics practices including proper handling of class imbalance, comprehensive evaluation metrics prioritizing recall for retention contexts, transparent model interpretation, and business-focused recommendations. Key findings reveal that month-to-month contracts have significantly higher churn rates (~43%) compared to one-year (~11%) and two-year contracts (~3%), with early tenure risk, fiber optic service issues, and payment method choice also serving as strong predictors of churn.

## Project Files
- [Notebook (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/telcom_churn/notebook.pdf)
- [White Paper (PDF)](https://github.com/dovkoy/msds-portfolio/tree/trunk/docs/projects/telcom_churn/white_paper.pdf)
