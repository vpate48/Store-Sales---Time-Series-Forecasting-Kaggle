Store Sales Time Series Forecasting
Introduction
This repository contains code for forecasting store sales using time series analysis. The goal is to predict future sales for various product families in different stores, taking into account factors such as promotions, holidays, and oil prices.

Dataset
The dataset used in this project consists of several CSV files:

train.csv: Contains historical sales data for training the model.
test.csv: Contains sales data for testing the model.
stores.csv: Contains information about the stores.
transactions.csv: Contains information about transactions in the stores.
holidays_events.csv: Contains information about holidays and events.
oil.csv: Contains historical oil prices.
Data Preprocessing
Merged relevant datasets to create a comprehensive dataset for analysis.
Handled missing values by replacing them with appropriate values.
Created additional features such as date-related features, lag features, rolling mean features, and exponentially weighted moving average features.
Model Building
Used CatBoost, a gradient boosting library, for building the forecasting model.
Split the dataset into training and validation sets.
Trained the model on the training data and evaluated its performance on the validation data.
Implemented a custom loss function, RMSLE (Root Mean Squared Logarithmic Error), to evaluate model performance.
Results
Achieved satisfactory performance on the validation set, as indicated by the RMSLE metric.
The trained model can be used to forecast store sales for future time periods.
