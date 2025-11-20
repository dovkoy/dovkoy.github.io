B"H

[← Back to Home](/)

# Bitcoin Price Movement Prediction Using Google Trends

## Research Question
Can Google Trends search data for cryptocurrency-related keywords be used to predict next-day Bitcoin price movement (up or down) with better-than-random accuracy?

## Project Overview
This project explores the relationship between public interest in cryptocurrency (measured through Google Trends) and Bitcoin price movements. The goal is to develop a binary classification model that predicts whether Bitcoin's price will increase or decrease the following day, providing actionable insights for short-term trading strategies.

The analysis encompasses three major components:

1. **Data Collection & Normalization** - Aggregating 10 years of daily Google Trends data for 5 cryptocurrency-related search terms ("bitcoin wallet", "crypto wallet", "buy crypto", "bitget", "buy bitcoin") using proxy rotation to bypass API limitations, and normalizing data across overlapping time windows
2. **Feature Engineering & EDA** - Cleaning and merging Bitcoin historical price data with Google Trends data, engineering technical indicators (RSI, MACD, Bollinger Bands), momentum features, rolling averages, and creating a binary target variable for next-day price direction
3. **Model Building & Evaluation** - Developing XGBoost classification models with GPU-accelerated hyperparameter tuning, comparing performance against naive baseline models, and evaluating predictive accuracy on held-out test data

The project demonstrates advanced data engineering techniques including proxy configuration for large-scale web data collection, time series normalization across discontinuous data windows, multivariate feature engineering, and machine learning model optimization for financial prediction tasks.

## Project Files
- [M1: Initial Problem Statement & EDA](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/predicting_btc/M1_Load_Normalize_Trends_BTC_Data.ipynb)
- [M2: Data Collection, Normalization & Preparation](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/predicting_btc/M2_Initial_EDA.ipynb)
- [M3: Model Building & Evaluation](https://github.com/dovkoy/dovkoy.github.io/tree/trunk/docs/projects/predicting_btc/M3_Model_Building_Eval.ipynb)
