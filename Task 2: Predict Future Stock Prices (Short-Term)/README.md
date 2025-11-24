# Task 2: Predict Future Stock Prices (Short-Term)

## Task Objective
Predict the next day's closing price of a selected stock using historical stock data.

## Dataset Used
- Source: Yahoo Finance (via `yfinance` Python library)
- Stock Example: Apple (AAPL)
- Features: Open, High, Low, Volume
- Target: Close price

## Models Applied
- Linear Regression
- Random Forest Regressor

## Key Results and Findings
- Linear Regression MSE: ~0.78 – captures overall price trends well.
- Random Forest MSE: ~26 – captures fluctuations but predictions are more volatile.
- Insights: Linear Regression provides stable short-term forecasts, while Random Forest may require tuning for improved accuracy. Visualization shows how predicted prices compare to actual closing prices.
