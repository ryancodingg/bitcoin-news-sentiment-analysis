# Bitcoin News Sentiment Analysis

# Bitcoin Price Prediction Analysis with Machine Learning

## Project Overview

This project analyzes historical Bitcoin price movements using machine learning techniques and time series forecasting models. It utilizes a dataset containing Bitcoin news headlines and price data over time. Various statistical and machine learning methods, such as ARIMA, Prophet, and feature engineering, are used to predict future Bitcoin prices and evaluate their performance.

The main goals of this project are:
- To perform exploratory data analysis (EDA) on Bitcoin price data.
- To apply machine learning models (e.g., ARIMA, Prophet) to predict Bitcoin price movements.
- To preprocess and transform text data from Bitcoin news headlines into numerical features using TF-IDF.
- To evaluate model performance using various metrics like MAE, RMSE, R-squared, and MAPE.

## Dataset Description

The dataset consists of historical Bitcoin price data and news headlines. It includes the following columns:
- **date**: The date of the data entry.
- **top_0, top_1, ... top_35**: News headlines related to Bitcoin.
- **price**: The closing price of Bitcoin on that date.
- **open**: The opening price of Bitcoin.
- **high**: The highest price of Bitcoin on that day.
- **low**: The lowest price of Bitcoin on that day.
- **vol.**: Trading volume for Bitcoin.
- **change %**: The daily percentage change in the Bitcoin price.

## Key Features

1. **Exploratory Data Analysis (EDA)**
   - Visualizations of historical price movements, distribution analysis, and price volatility.
   - Statistical analysis of the price, volume, and price change percentage.
   - Correlation analysis between Bitcoin price and volume.

2. **Time Series Decomposition**
   - Seasonal decomposition of time series data to capture trends, seasonality, and residuals.

3. **Feature Engineering**
   - Generation of technical indicators like the Relative Strength Index (RSI) and moving averages (SMA, EMA).
   - Text data processing (headline text) using TF-IDF (Term Frequency-Inverse Document Frequency) to generate numerical features for the models.

4. **Modeling**
   - **ARIMA**: Autoregressive Integrated Moving Average model for time series forecasting.
   - **Prophet**: A forecasting model designed for time series data with daily seasonality.
   - **ARIMAX**: ARIMA with exogenous variables such as TF-IDF features extracted from the Bitcoin headlines.

5. **Evaluation**
   - Evaluation of models using performance metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Percentage Error (MAPE), and R-squared.

## Requirements

To run this project, you will need the following Python packages:
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels
- sklearn
- prophet
- nltk
- textblob
- scipy

You can install all required packages by running:

pip install -r requirements.txt


