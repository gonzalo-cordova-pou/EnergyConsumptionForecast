# Energy Consumption Forecast

[![Python 3.10](https://img.shields.io/badge/python-3.10-blue)](https://www.python.org/downloads/release/python-3100/) 

![Alt text](image.png)

I wanted to learn more about XGBoost and how it can be used to forecast energy consumption. I found a dataset on Kaggle that had hourly energy consumption data for a year. I used this dataset to train an XGBoost model to forecast energy consumption. I used the `xgboost` library in Python to train the model. I used `matplotlib` and `seaborn` to visualize the results.

The material provided is a selection of different notebooks that I used to learn about XGBoost and is not claimed to be original work. Check out the references section for links to the original material.

## Dataset

The dataset I used is from Kaggle. It can be found [here](https://www.kaggle.com/robikscube/hourly-energy-consumption). The dataset contains hourly energy consumption data for a year. The data is from PJM Interconnection LLC, a regional transmission organization (RTO) in the United States. The data is from 2002 to 2018. The dataset contains the following columns:

* `Datetime`: The date and time of the energy consumption data
* `PJME_MW`: The actual energy consumption in megawatts

## Notebook

The notebook can be found [here](EnergyConsumptionForecast.ipynb). The notebook contains the following sections:

- Loading the data
- Outlier removal
- Simple training method
    - Train/test split
    - Feature creation
    - Visualize our Feature / Target Relationship
    - Create and Train our Model
    - Feature Importance
    - Forecast on Test
    - Score (RMSE)
    - Calculate Error
- Time Series Cross Validation (+ using lag features)
    - Forecasting Horizon Explained
    - Lag Features
    - Training
    - Predicting the future
- Saving and loading the model

## Other methods
Despite having tried XGBoost, other methods could be tried (I will soon :)):
- LSTM model. Check out: [TensorFlow-Time-Series-Examples](https://github.com/hzy46/TensorFlow-Time-Series-Examples/blob/master/train_lstm.py)
- (S)ARIMA models. Check out an example using the `statsmodels` Python library [here](https://www.kaggle.com/code/mariavirginiaforcone/power-consumption-forecasting-with-sarima-tbats)
+ extra: interesting paper by Dubey et al.: [Study and analysis of SARIMA and LSTM in forecasting time series data](https://www.sciencedirect.com/science/article/pii/S2213138821004847?casa_token=aX5EMq_LZqMAAAAA:Qgjd4Ei4VvC6ZzO-jm-75AbzgaCN1EGEb1xu7WxOmz2wvBSPgQQW0ip4v7rucViyi51Bf_N_lu0)

## References

* [XGBoost Documentation](https://xgboost.readthedocs.io/en/latest/)
* [XGBoost Paper](https://arxiv.org/abs/1603.02754)

Most of the material I used in this notebook came from the following notebook by [Rob Mulla](https://www.kaggle.com/code/robikscube/time-series-forecasting-with-machine-learning-yt). Check out his YouTube channel [here](https://www.youtube.com/@robmulla).
