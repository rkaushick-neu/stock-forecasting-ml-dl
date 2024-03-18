# Stock Forecasting Project using ML & DL Techniques
This project uses Machine Learning &amp; Deep Learning regression techniques to forecast the S&amp;P 500 stock prices.

## Project PDF Report
You can find the report to this project by clicking [here](/Rish_Stock_Forecasting_Project_Report.pdf) or navigating to the 'Rish_Stock_Forecasting_Project_Report.pdf' file in this repository.

## Simpler Models Branch
In this branch, I removed the feature engineering steps (like calculating price % change, moving average and Clustering) to see how it compares. I understood that the previous models with extensive feature engineering were more difficult to generalize. The same models (with same hyper-parameters) were trained on the data without the feature engineering and surprisingly performed much better.

Please find below the comparison graphs for all models:

![Random Forest models comparison graphs](/img/rf_regressor_graphs.png)
![XG Boost models comparison graphs](/img/xgb_regressor_graphs.png)
![LSTM models comparison graphs](/img/lstm_graphs.png)

## My Learning
Specifically in this scenario, interestingly, I noticed that the models which were trained on data without significant feature engineering performed much better than their counter parts. 
The reasons for this could be:
1. Overfitting: feature engineering by adding too many features or complex transformations can sometimes lead to overfitting.
2. Loss of information: Perhaps the dimensionality reduction of PCA + Clustering for feature engineering may have resulted in loss of original information because of which the model does not generalize well.
3. Ineffective features: The features that I chose may not have been as relevant as I intended. 
