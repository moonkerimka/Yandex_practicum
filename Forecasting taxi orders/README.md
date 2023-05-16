## Predicting the number of taxi orders at a certain hour

### Tool stack

Time series processing, statsmodels library;
Analysis of the global trend, seasonality, daily and hourly patterns;
feature engineering: splitting the date into components, introducing lags and moving averages;
sklearn and gradient boosting models - CatBoost, LightGBM;
Selection of model hyperparameters using hyperopt.

### Input data

Taxi aggregator analyzes patterns in daily orders to attract more drivers during peak hours.

There is labeled data: the number of orders per hour for several months.

### Target

Build a model to predict the number of orders per hour. The prediction time and RMSE metric should be kept to a minimum.

### Project structure

1. Downloading data and resampling for one hour;
2. Data analysis: trends, seasonality, data type, anomaly search;
3. Training and validation of models;
4. Checking models on a test sample and drawing conclusions.
### Conclusion
📑A study was conducted to predict taxi orders.

Input data - historical data about taxi orders at airports.


📊 The time series is stationary. The trend shows a linear increase in the number of orders over time.


📊 Linear regression, random forest, decision tree, XGBoost, CatBoost, LightGBM, lasso regression and ridge regression models were trained.


📊 Found the best hyperparameters for the respective models using GridSearchCV.


📊 A comparison of the quality of the studied models using the RMSE metric on the validation set is shown.


Based on the analysis, the conclusion is made:
- the best model with lower RMSE is lasso regression.
- Gradient boosting and Decision Tree models became the worst model.
