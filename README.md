# Anomaly Detection: Rim Cleaning Machine Use Case

## Bachelor Thesis
[Anomaly Detection Using Time Series Analysis for Vibration Signals](https://github.com/DarjaStrahl/PredictiveMaintenance/blob/master/document.pdf) - Darja Strahlberg, Bachelor Thesis, TUHH 2020

The overall structure is composed of 3 parts: an ARIMA model for forecasting the vibration signal, Confidence Interval build in the correlation to the forecast and an evaluation of data points lying outside of the confidence interval. 

## Dependencies
```Python == 3.7, numpy, statsmodels```

## Explanation
The file `Test1Day.ipynb` evaluates data, collected during one day, with the frequency 1 minuted. ARIMA forecast for 60 data points, 1 hour, confidence interval are computed. No anomaly was identified.

The file `Test1Day_night.ipynb` evaluates data, collected during one day, with the frequency 1 minuted. ARIMA forecast for 200 data points, 3 hours, confidence interval are computed. Anomaly, as a state of the pump in the night, was successfully identified.

The file `Test1Day_characterisation.ipynb` evaluates data, collected during one day, with the frequency 1 minuted. Autocorrelation, partial autocorrelation plots and a seasonal decomposition are computed. 

The file `ComparativeAnalysis.ipynb` evaluates data, collected during one day, with the frequency 1 minuted. Different forecast methods are computed: mean, simple average and etc.  

The file `ARIMA_choosing.ipynb` evaluates data, collected during one day, with the frequency 1 minuted. Grid search for the best parameter evaluation for ARIMA. 

## How to Run
Load the data, click run in the jupiter Notebook to excetute cells and show the results. 
