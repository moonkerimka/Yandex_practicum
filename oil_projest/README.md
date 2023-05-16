## The choice of locations for wells

### Tool stack

Development of the boostrap technique;
Work with business metrics: gross, operating, net profit, conversions, online and offline indicators;
seaborn visualization.
### Input data

An oil producing company hires a specialist to analyze the profitability of oil fields. We have information about the deposits from the exploration team. Well development budget is limited. You need to select the region and wells with the maximum oil reserves to maximize profits.

There are labeled data: information about deposits and approximate oil reserves.

### Target
Select the region with the maximum profit from oil production.

### Project structure
Load and preprocess data.
Train and test the models: 
2.1. Train the model and make predictions on the validation set for each region; 
2.2. Printed on the screen is the average stock of raw materials and the RMSE model; 
2.3. Analyze results.
Prepare available data: 
3.1. Calculate the minimum average volume of raw materials in the deposits of the region, sufficient for its development. draw conclusions; 
3.3. Write a function to calculate profit for a set of selected fields and model predictions.
Calculate risks and profits for each region: 
4.1. Apply the Bootstrap technique; 
4.2. Find the average profit, 95% confidence interval and risk of loss; 
4.3.Choose the best region for mining.

### Conclusion  
A linear regression model was trained. A prediction function based on the trained model is written, then it is cast to Series and indexes are set.


The volume of raw materials for the break-even development of a new well is 111, but the volume of reserves of an average well in the regions is much less than this value: 92.5, 68.83, 95. The average reserve of the region of the second region (68.8) is much less than that of other regions and the calculated reserve for break-even field development (111).


A function is shown in which 1000 samples are generated to find the profit distribution. The average return, 95% confidence interval, risk of loss, and profit distribution for the three regions are shown as predicted by the linear regression model. The best forecast is given by the second region, because the risk of loss is only 2%. The worst forecasts were shown by the first and third regions - 6.7 and 7.4%.


Based on this, the conclusion is made:
- the second region is proposed for choosing the location of the well, because the risk of loss is small.

