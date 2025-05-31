WTI Crude Oil Price Forecasting with ARIMA
Overview
This project focuses on forecasting the daily closing price of West Texas Intermediate (WTI) crude oil futures using time series analysis with ARIMA models. The goal is to build a baseline predictive model, optimize its parameters, and validate its performance through walk-forward validation and residual diagnostics.

Dataset
Source: Yahoo Finance (CL=F ticker)
Frequency: Daily closing prices

Objectives
Download and preprocess WTI daily closing price data
Explore and optimize ARIMA model parameters (p, d, q) using grid search
Perform walk-forward validation for robust evaluation
Analyze residuals to check model assumptions (stationarity, white noise)
Visualize results: actual vs predicted prices, residual plots, ACF, QQ plots
Report model performance metrics (RMSE, R²)

Methodology
Data Preparation:
Extract and clean daily closing prices, split into training (80%) and test (20%) sets.

Model Selection:
Use grid search over ARIMA parameters (p=0-5, d=0-2, q=0-5) to find the best model minimizing RMSE.

Walk-Forward Validation:
Iteratively forecast each point in the test set, updating the training history with actual observations.

Residual Diagnostics:
Validate model assumptions by analyzing residual plots, autocorrelation (ACF), and conducting Ljung-Box tests.

Results
Best ARIMA model order found: (p, d, q) with lowest RMSE.
Model explains significant variance and captures temporal dependencies.
Residual analysis confirms residuals behave approximately like white noise, validating the model.

Potential Improvements
Incorporate exogenous variables (Brent prices, USD index, geopolitical indicators)
Explore non-linear models (Random Forests, XGBoost, LSTM)
Develop multi-step ahead forecasting models
Add technical indicators as features (RSI, MACD, momentum)

Usage
Ensure dependencies are installed: pandas, numpy, matplotlib, statsmodels, yfinance, scikit-learn
Run the Jupyter notebook or Python scripts to reproduce data download, modeling, and visualization.

License
This project is licensed under the MIT License.
  
