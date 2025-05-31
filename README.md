# time-series-forecasting-WTI
Basic analysis and forecasting of WTI crude oil prices using time series models such as ARIMA and Linear Regression.
This project explores various time series analysis and modeling techniques to predict the daily closing prices of West Texas Intermediate (WTI) crude oil futures (ticker CL=F).

Objective
The main goal is to apply and compare multiple modeling approaches, ranging from linear regression with time-based features to classical ARIMA models, to evaluate their effectiveness for short-term forecasting of WTI prices. The project also covers exploratory data analysis, feature engineering, and diagnostic model analysis.

Data Used
Historical WTI crude oil futures price data (ticker CL=F) were downloaded using the yfinance library.
Ticker: CL=F


Methodology
The project follows these steps:
Data Acquisition: Download data from Yahoo Finance.
Cleaning and Inspection: Check for missing values, data types, descriptive statistics.

Feature Engineering:
Create lags (past price values).
Create rolling windows (moving averages, rolling standard deviations).

Modeling:
Linear Regression: Using various combinations of lags and rolling window features.
Lag/Window Optimization: Iterative search for best parameters in linear regression.
ARIMA: Iterative search for optimal (p, d, q) based on RMSE. 
  Walk-forward validation. 
  Residual Analysis.
  Check residuals for white noise behavior (plots, Ljung-Box test).
  Check normality (histogram, Q-Q plot).
  
