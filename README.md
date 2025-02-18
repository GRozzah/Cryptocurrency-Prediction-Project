# Cryptocurrency Analysis and Prediction

This project performs cryptocurrency data analysis and prediction using machine learning and time series forecasting techniques. It focuses on gathering, cleaning, and transforming historical cryptocurrency data, followed by applying various models for predicting future trends.

## Table of Contents

- [Overview](#overview)
- [Libraries Used](#libraries-used)
- [Data Collection](#data-collection)
- [Data Cleaning and Transformation](#data-cleaning-and-transformation)
- [Modeling](#modeling)
- [Results](#results)
- [Future Work](#future-work)

## Overview

The goal of this project is to analyze and predict the prices of major cryptocurrencies such as Bitcoin (BTC), Ethereum (ETH), and others using historical price data. By using machine learning techniques, this project aims to forecast the price trends of these cryptocurrencies.

Key features:
- Data collection from Yahoo Finance API
- Data cleaning, missing value handling, and feature engineering
- Time series analysis with ARIMA and LSTM models
- Visualization using Plotly and Matplotlib
- Exporting transformed data for further analysis

## Libraries Used

The following libraries are used in this project:

- `yfinance` for downloading historical cryptocurrency data
- `pandas` for data manipulation
- `matplotlib` and `seaborn` for visualization
- `scipy` for statistical analysis
- `sklearn` for machine learning models (PCA, KMeans, ARIMA)
- `tensorflow.keras` for LSTM model
- `statsmodels` for time series analysis
- `plotly` for interactive visualizations
- `streamlit` for building interactive web apps

## Data Collection

Data is collected using the `yfinance` library, which retrieves historical market data for the following cryptocurrencies:
- Bitcoin (BTC-USD)
- Ethereum (ETH-USD)
- Ripple (XRP-USD)
- Litecoin (LTC-USD)
- Bitcoin Cash (BCH-USD)

The data is collected for a specified time period and is then preprocessed for further analysis.

## Data Cleaning and Transformation

In this step, we clean the collected data:
- Missing values are handled using forward fill (`ffill`).
- Duplicate rows based on the 'Date' index are removed.
- The data is transformed into a format where each cryptocurrency is represented by its closing price over time.
- The data is saved to a CSV file for future use or export.

## Modeling

We employ both statistical and machine learning models to forecast cryptocurrency prices:
1. **ARIMA**: A time series forecasting model used to predict future prices based on past trends.
2. **LSTM (Long Short-Term Memory)**: A deep learning model used for time series forecasting, particularly suited for sequential data like cryptocurrency prices.

## Results

The project outputs include:
- Visualizations of cryptocurrency price trends and forecasts
- Transformed and cleaned data saved to a CSV file for further analysis

## Future Work

- Improve model accuracy by tuning hyperparameters and incorporating additional features (e.g., sentiment analysis, macroeconomic data).
- Explore other advanced machine learning techniques like XGBoost or Prophet for better forecasting.
- Deploy the model in a real-time forecasting application using Streamlit.


