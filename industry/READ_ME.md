## Industry

### Tool stack

CatBoost, Random Forest, Desicion Tree, Linear Regression, XGBoost, LightGBM.
### Input data

historical data of the metallurgical plant "Tak Temper Steel". An exploratory data analysis was carried out to examine the data. Input data - historical data of the metallurgical plant LLC "So we temper steel". 

### Target
To build a model that predicts the temperature of steel.

### Conclusion  
📊 The data was pre-processed as follows: the names of the columns were corrected; empty lines are filled; data in columns changed; some columns are removed because they are not informative; added column with full power.


📊 Data standardization has been carried out.


📊 Linear regression, random forest, decision tree, XGBoost, CatBoost, LightGBM models were trained.


📊 Found the best hyperparameters for the respective models using GridSearchCV.


📊 The studied models behave in a similar way and select the same features as the most important, such as "key", "Start_temperature", "Wire_1".


📊 Comparison of the quality of the studied models using best_score is shown.


Based on the analysis, the conclusion is made:
- the best CatBoost model, then LightGBM, after XGBoost.
- the worst model of Linear Regresion, Random Forest and Decision Tree, they have the lowest best_score.
