WTI Crude Oil Price Forecasting with ARIMA
---
Overview:
This project focuses on forecasting the daily closing price of West Texas Intermediate (WTI) crude oil futures using ARIMA time series models. The objective is to build a baseline predictive model, optimize its parameters, and validate its performance through walk-forward validation and residual diagnostics.

Dataset:
Source: Yahoo Finance (CL=F ticker) - Frequency: Daily closing prices

Objectives:
Download and preprocess WTI daily closing price data
Explore and optimize ARIMA parameters (p, d, q) using grid search
Perform walk-forward validation for robust model evaluation
Analyze residuals to verify model assumptions (stationarity, white noise)
Visualize results including actual vs predicted prices, residual plots, ACF, and QQ plots
Report model performance metrics such as RMSE and R²

Methodology:
Data Preparation
Extract and clean daily closing prices, then split the data into training (80%) and test (20%) sets.

Model Selection:
Conduct a grid search over ARIMA parameters (p=0-5, d=0-2, q=0-5) to identify the best model minimizing RMSE.
Walk-Forward Validation
Iteratively forecast each point in the test set while updating the training history with observed values.

Residual Diagnostics:
Validate model assumptions by analyzing residual plots, autocorrelation function (ACF), and performing the Ljung-Box test.

Results:
Best ARIMA model order (p, d, q) identified with lowest RMSE
Model effectively captures temporal dependencies and explains significant variance
Residual analysis indicates residuals behave like white noise, confirming model adequacy

Usage, Install required dependencies:
pandas, numpy, matplotlib, statsmodels, yfinance, scikit-learn
Run the provided Jupyter notebook or Python scripts to reproduce data download, modeling, and visualization.

License
This project is licensed under the MIT License.
