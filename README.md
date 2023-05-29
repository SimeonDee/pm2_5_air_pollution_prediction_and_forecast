# pm2_5_air_pollution_prediction_and_forecast
Analysis of Air Pollution prediction and time-series forecast of PM2.5 Pollutant using Machine Learning Algorithms (SVM, Decision Tree and Random Forest) and Deep Learning Algorithms (CNN and Bi-LSTM).


## Dataset Source
- [Beijing Multi-Site Air Quality Dataset: UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Beijing+Multi-Site+Air-Quality+Data#)

- Only Nongzhanguan and Gucheng stations Air Quality Data were used in this work


## Three (3) Forecast Models were built each one based on the following:
Lags: 24 hours

1. Univariate Time Series: Considering only the past 24 lags of PM2.5, 
2. Multi-input Time-Series: Considering all exogenous weather variables (past 24 lags) to forecast future PM2.5
3. Multi-input Time-Series: Considering selected (based on pearson correlation) exogenous weather variables (past 24 lags) to forecast future PM2.5

Forecasts were made for 24 hours, 1 week and 1 month into the future for each algorithms

Also considered for improved performances is random search hyper-parameter tuning using Ray-Tune with HyperBand Scheduler strategy.

