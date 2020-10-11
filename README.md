# Time_Series_Janta_Hack
This repository contains the code for the Analytics Vidhya Time Series Prediction Hackathon. The dataset can be found [here](https://datahack.analyticsvidhya.com/contest/janatahack-time-series-forecasting/#About).

The competition was about the prediction of the electricity consumption of a user for the end week of every month. An hourly data of electricity consumption along with other variables was provided for 1st to 24th of every month as training data and similar observations for all other variables, except electricity consumption, were provided for 24th to 30th or 31st of every month as testing data.

The metric for evaluation was root mean square error.

Out of all the models, the **CatBoost** model gave the best rmse score for the validation data.

Before applying feature engineering on the 'electricity_consumption' column, our model performed better and gave the following results.
The model results were as follows:(public score,private score)

* XGBoost: 81.7951,99.1029
* LightGBM: 91.88575,98.4433
* CatBoost: 75.6317, 97.9808

We also tried creating datetime features like quarter of year,weekday or weekend, day of week but they increased the model rmse score.
