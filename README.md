# Air Quality Forecasting using Prophet and ARIMA

This project focuses on forecasting various air quality indicators using Facebook Prophet and ARIMA models. The dataset includes hourly data on pollutants and weather parameters.

##  Features
- Time series preprocessing and handling missing values
- Forecasting 13 variables (CO, NOx, T, RH, etc.)
- RMSE calculation on last 10% of data
- Comparison of model performance against predefined thresholds

##  Models Used
- Facebook Prophet
- ARIMA

##  Files Included
- `prophet_forecast.py` – Builds and evaluates Prophet models
- `arima_forecast.py` – ARIMA modeling for each variable
- `rmse_comparison.txt` – Final RMSE vs Threshold comparison
- `requirements.txt` – Python dependencies

##  Evaluation Summary
A text summary is available in `prophet_rmse_comparison.txt` showing which variables meet performance criteria.

##  Installation
```bash
pip install -r requirements.txt
```

##  Author
Ramanuja Prabu – CSE Student | 2nd Year 
