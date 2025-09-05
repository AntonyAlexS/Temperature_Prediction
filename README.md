📖 Project Overview

This project focuses on predicting temperature using humidity data collected from multiple IoT sensors. The dataset contains over 700,000 records with features such as:

sensor_id
lat, lon (sensor location)
pressure
temperature (target variable)
humidity (main feature used for prediction)

The goal is to explore the dataset, handle outliers, preprocess features, and build regression models to predict temperature.

🔎 Steps Followed
1. Exploratory Data Analysis (EDA)
Inspected dataset shape, column types, duplicate values and missing values.
Checked distributions of temperature, humidity, and pressure.
Identified and treated outliers using IQR method.
Analyzed correlation between variables (humidity vs temperature showed a stronger relationship).

2.Data Preprocessing
capped outliers in temperature and pressure.
Train-test split (80% training, 20% testing).

3. Model Building
Linear Regression
Polynomial Regression

4.Model Evaluation Metrics
MAE (Mean Absolute Error)
RMSE (Root Mean Squared Error)
R² Score

Conclusion:
Polynomial Regression with degree 2 achieved the best balance of accuracy, showing the highest R² and lowest error. After hyperparameter tuning, degree 4 provided a slight improvement, but the difference was not significant. Therefore, Polynomial Regression (degree 2 or 4) is recommended for predicting temperature from humidity in this dataset.