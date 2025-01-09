# Bitcoin News Sentiment Analysis

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


``` bash
pip install -r requirements.txt
```

## Getting Started

1. **Clone the repository**:
``` bash
git clone https://github.com/your-username/bitcoin_news_sentiment_analysis.git
```

2. **Navigate to the project folder**:
``` bash
cd bitcoin-news_sentiment_analysis
```

3. **Install dependencies**:
``` bash
pip install -r requirements.txt
```

4. **Run the Jupyter Notebook**:
- Open the Jupyter Notebook:
  ```
  jupyter notebook
  ```
- Run `bitcoin_news_sentiment_analysis.ipynb`.

## Results

- **Model Performance**: The best model (e.g., Prophet, ARIMA) achieved an R-squared value of 0.90, indicating strong prediction accuracy. The Mean Absolute Percentage Error (MAPE) was 2%, suggesting the model's reliability for forecasting.
- **Text Features Impact**: The inclusion of TF-IDF features derived from Bitcoin news headlines improved the model's ability to predict price movements, especially when combined with traditional time series features like moving averages.

## Conclusion

This project demonstrates how machine learning models can be used to predict Bitcoin prices by combining time series forecasting methods with text data analysis. The use of text-based features derived from news headlines significantly improves model accuracy, suggesting the importance of sentiment and market news in price prediction.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [Bitcoin Historical Data Source](https://www.kaggle.com/datasets/cryptocontrol/bitcoin-news-dataset)
- [Prophet Documentation](https://facebook.github.io/prophet/)
- [ARIMA Documentation](https://www.statsmodels.org/stable/generated/statsmodels.tsa.arima.model.ARIMA.html)





