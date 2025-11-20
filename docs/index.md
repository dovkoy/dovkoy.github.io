---
layout: default
---

B"H

# Data Science Portfolio

Welcome! I'm David Koyrakh, a computer and data science professional passionate about bringing valuable design and energy to your team.

<p>
  <em>
    Hint: You can find the complete source code and projects on my 
    <a href="https://github.com/dovkoy/dovkoy.github.io/" target="_blank">GitHub repository</a>.
  </em>
</p>


* * *

## About

My expertise includes full-stack engineering, machine learning, and big data pipelines. I like to experiment with predictive modeling to identify patterns hiding in publically-available data (there's a lot out there!) such as cryptocurrency price trends and search engine data. Currently, I work as a freelance software engineer.

My experience spans various domains including AI, SaaS, finance, medical tech, telecom, and more.

### Skills & Technologies

**Programming Languages:** Python, JavaScript and TypeScript, R, SQL

**Machine Learning:** Random Forest, Neural Networks, Deep Learning

**Big Data:** Hadoop, Spark, HBase, Kafka, NiFi, Kubernetes

**Data Visualization:** Matplotlib, Seaborn, ggplot2, Tableau, Power BI

**Cloud Platforms:** AWS, Google Cloud Platform

**Statistical Analysis:** Hypothesis Testing, Regression Analysis, Time Series, Clustering

**Tools & Frameworks:** Git, Docker, Jupyter, pandas, NumPy, Scikit-learn, TensorFlow

### Education

**Master of Science in Data Science**  
Bellevue University

### What I'm Looking For

I'm seeking opportunities to leverage data science and machine learning to solve challenging business problems, particularly in finance (traditional or crypto). I'm passionate about creating interpretable, ethical AI solutions that deliver impact.

* * *

## Projects

Below are some of the key projects I've worked on, demonstrating my skills across various aspects of data science:

### 1. Bitcoin Price Prediction Using Google Trends

Developed a binary classification model predicting next-day Bitcoin price movement (up or down) by combining 10 years of Google Trends search data for cryptocurrency-related keywords with technical indicators (RSI, MACD, Bollinger Bands). Implemented advanced data engineering including proxy rotation for large-scale data collection, time series normalization across overlapping windows, and GPU-accelerated XGBoost hyperparameter tuning, achieving 54% validation accuracy above random baseline.

**Link:** [View Project](/projects/predicting_btc/readme.md)

---

### 2. Multi-Source Data Analysis of U.S. State Statistics

Demonstrated end-to-end data integration from three distinct sources (USDA labor statistics, Wikipedia religiosity data, and U.S. Census API) to create a comprehensive state-level dataset. Implemented data extraction, transformation, and storage in SQLite with aggregate analysis and visualization showcasing patterns across economic, demographic, and social factors.

**Link:** [View Project](/projects/multi_source_data_analysis/readme.md)

---

### 3. Big Data Pipeline: Advertisement Performance Analysis

Orchestrated a complete big data pipeline using Apache NiFi, HDFS, Hive, Spark (via YARN), and HBase to ingest, store, process, and analyze online advertisement performance data. Built and evaluated a Linear Regression model using Spark MLlib to predict revenue from advertising metrics, demonstrating end-to-end workflow orchestration across multiple big data technologies with Docker container management and distributed computing.

**Link:** [View Project](/projects/big_data_pipeline/readme.md)

---

### 4. U.S. Childcare Cost Analysis Dashboard

Analyzed the National Database of Childcare Prices to reveal geographic and economic disparities in U.S. childcare costs. Created an interactive HTML/JavaScript dashboard with D3.js featuring choropleth maps showing costs as percentage of median household income by county, with filtering capabilities for age groups and care types. Developed supporting infographics and presentation materials for policymakers, revealing that national average affordability (15.9% of income) exceeds the federal benchmark of 7%.

**Link:** [View Project](/projects/child_care_cost/readme.md)

---

### 5. Telecom Customer Churn Prediction Model

Developed a predictive model for the IBM Telco Customer Churn dataset (7,000+ customers) using class-weighted Logistic Regression to identify customers at risk of leaving their telecom provider. Achieved ROC-AUC of 0.846 with 80% recall, capturing 8 out of 10 churners. Identified contract type as the strongest predictor, with month-to-month contracts showing 43% churn rate compared to 3% for two-year contracts, providing actionable insights for retention strategies.

**Link:** [View Project](/projects/telcom_churn/readme.md)

---

### 6. Titanic Survival Analysis with R

Conducted rigorous statistical analysis of RMS Titanic disaster data (887 passengers) to investigate how socioeconomic factors influenced survival outcomes. Evaluated multiple data sources, performed comprehensive EDA answering five research questions, and developed a logistic regression model using R to quantify the impact of passenger class, fare, family size, age, and gender on survival probability.

**Link:** [View Project](/projects/titanic_survival_factors/readme.md)

---

### 7. AI Customer Service Agent Escalation Failure Mitigation

Developed a production-grade safeguard for AI customer service systems to reliably catch failed escalations. The system detects when an agent claims to transfer a user to a human representative, but the actual escalation is not triggered. Implemented a two-layer defense: fast keyword filtering and an optional LLM-based binary classifier using OpenAI's Structured Output API. Comprehensive unit tests ensure reliability across a wide range of message scenarios.

**Link:** [View Project](/projects/agent_escalation/readme.md)

---

### 8. Ames Housing Price Prediction

Built transparent and performant regression models to predict home sale prices in Ames, Iowa using the widely-used Ames Housing dataset (1,460 properties with 79 features). Compared Ridge regression, Random Forest, and Gradient Boosting approaches with comprehensive feature engineering and missing value handling. Achieved best performance with Gradient Boosting (RMSE ≈ $28.4K, R² ≈ 0.851), identifying overall quality and living area as dominant price drivers through correlation analysis and tree-based importance metrics.

**Link:** [View Project](/projects/ames_home_prices/readme.md)

---

### 9. Census Income Prediction and Socioeconomic Analysis

Developed interpretable models using the Adult Census Income dataset (32,561 records from 1994 U.S. Census) to predict whether an individual's annual income exceeds $50,000. Trained Logistic Regression and Random Forest models inside leak-safe pipelines, achieving ROC-AUC ≈ 0.90 on held-out data. Identified capital gain, marital status, education, hours worked, and age as key income drivers, with comprehensive subgroup evaluation revealing performance differences across demographics that inform fairness-aware deployment considerations.

**Link:** [View Project](/projects/adult_census_income/readme.md)

---

### 10. Heart Disease Risk Prediction for Clinical Decision Support

Developed an interpretable, end-to-end analysis for predicting heart disease presence using the UCI Heart Disease dataset (Cleveland subset, 304 records). Trained Logistic Regression and Random Forest models with class-balanced weighting, achieving strong discrimination (Logistic Regression: ROC-AUC 0.936, Random Forest: ROC-AUC 0.952 on single split; RF cross-validation: ROC-AUC ≈ 0.915). Extracted clinically sensible risk drivers including chest pain presentation, vessel count, and ST/thal findings to support preventative care and early intervention decisions.

**Link:** [View Project](/projects/heart_health/readme.md)

* * *

## Contact

I'm always interested in connecting with fellow data enthusiasts, potential collaborators, and employers. Feel free to reach out!

**LinkedIn:** [linkedin.com/in/davidkoyrakh](https://www.linkedin.com/in/davidkoyrakh/)

**GitHub:** [github.com/dovkoy](https://github.com/dovkoy)

---

_Last updated: November 2025_
