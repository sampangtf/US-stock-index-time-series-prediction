# US-stock-index-time-series-prediction


Stock Indices are important indicators of the financial market performances as they aggregate the price movements of the most prominent companies with the highest market capitalizations. They are the proxy metrics of economic prosperity and informs the corporate and individual investors on decisions in asset and portfolio management. 

This project aims to model the movement of the monthly S&P 500 and Dow Jones Industrial Average (DJIA) by conducting univariate modeling against their past time series data between 1992 and 2020 (inclusive), as well as investigate the effect of macro-economic variables through multivariate analysis of DJIA. Our team has developed 7 univariate models and 5 multivariate models to predict the stock indices, including the conventional time series models (ARIMA, GARCH, VAR, etc.) and new-found deep learning models (LSTM, Transformers). 

We extracted our indices data from Bloomberg, performed data cleaning and integration with macro-economic factors and exploratory data analysis in terms of stationarity and cross-correlation. We trained most of our models mostly on original time series and some in differenced time series due to the model assumption. 

Based on the goodness of fit metrics from residual analysis, and prediction evaluation metrics, we compared different model’s performance, found that: 
    1. multivariate model does not necessary outperform univariate model; 
    2. ARMA-GARCH and eGARCH have the best predictive power with less-than-one Precision Error (PM) despite the limitation in short-run flat predictions and those from ARIMA/SARIMA follows the movement and keep up with the changes ; and 
    3. Prophet and LSTM might be particularly good in dealing with predicting time series with shocks.