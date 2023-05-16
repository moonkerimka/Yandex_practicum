## Determination of the price of the car according to the available characteristics

### Tool stack

Data preprocessing: processing of omissions and duplicates, changing the data type, grouping tables;
Application of gradient boosting models: sklearn, LigtGBM, XGBoost, CatBoost, Decision Tree, Random Forest, Linear Regression;
Model validation.
### Input data

A used car sales service is developing a mobile application. The algorithm determines the cost of the car put up for sale.
The model should give the most accurate price, learn quickly and have a minimum prediction time.

### Target

Create a model that predicts the price of a car based on certain features.

Labeled data available: vehicle characteristics and sales price

### Project structure

1. Loading and processing data: filling gaps, grouping by detection, searching for duplicates, visualizing results;
2. Training of gradient boosting models, learning rate analysis;
3. Checking models and choosing the best version for launch in production.

### Conclusion  
Scaled and standardized data.
Linear regression, random forest, decision tree, XGBoost, CatBoost, LightGBM models were trained.
Found the best hyperparameters for the respective models using GridSearchCV.

A comparison of the quality of the studied models using the RMSE metric, as well as training and prediction times is shown.


Based on the analysis, the conclusion is made:
- the best CatBoost model, then LightGBM, after Random Forest.
CatBoost is the fastest training and prediction model for gradient boosting compared to LightGBM and XGBoost.
is the worst Linear Regression model, it has the highest RMSE metric.

