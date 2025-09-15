# Smart Cab 

This machine learning project focuses on predicting "cab fare amount", "fuel consumption", and "combustion energy" based on various trip-related features. It uses regression techniques to build predictive models on a real-world dataset, applying effective data preprocessing, feature engineering, and model evaluation methods.



# Project Objectives

* Predict "fare amount" based on trip details like distance, time, and pickup/drop-off locations.
* Estimate "fuel consumption" using trip duration and environmental factors.
* Calculate "combustion energy" required per trip, considering fuel efficiency metrics.
* Apply machine learning techniques to create accurate, explainable models.



# Machine Learning Techniques Used

* Exploratory Data Analysis (EDA) with `matplotlib`, `seaborn`, and `pandas`

--> Feature Engineering:
  * Distance calculation using geolocation (Haversine formula)
  * Time-based features (hour of day, day of week)

--> Data Preprocessing:
  * Handling missing values and outliers
  * Feature scaling (StandardScaler / MinMaxScaler)

--> Modeling:
  * Linear Regression
  * Random Forest Regressor
  * XGBoost Regressor
  * Gradient Boosting

  ** Models were trained on the processed training data and evaluated using:

- Root Mean Squared Error (RMSE)
- R² Score (Coefficient of Determination)
    
--> Evaluation Metrics:
  * RMSE, MAE, R² Score



# Dataset Overview

--> The dataset includes the following key features:

| Column Name        | Description                                 |
|--------------------|---------------------------------------------|
| "pickup_datetime"  | Timestamp of the ride start                 |
| "pickup_longitude" | Pickup location longitude                   |
| "pickup_latitude"  | Pickup location latitude                    |
| "dropoff_longitude"| Drop-off location longitude                 |
| "dropoff_latitude" | Drop-off location latitude                  |
| "passenger_count"  | Number of passengers                        |
| "fare_amount"      | Fare charged for the trip (target)          |
| "trip_distance"    | Distance traveled (engineered feature)      |
| "fuel_consumption" | Predicted fuel consumption (target)         |
| "combustion_energy"| Estimated combustion energy (target)        |



# Result Summary

| Model                   | RMSE (Train) | R² Score (Train) | RMSE (Test) | R² Score (Test) |
| ----------------------- | ------------ | -----------------| ----------- | --------------- |
| Linear Regression       | 0.25         | 0.77             | 0.24        | 0.79            |
| Decision Tree Regressor | 0.29         | 0.70             | 0.28        | 0.72            |
| Random Forest Regressor | 0.093        | 0.97             | 0.24        | 0.79            |
| Gradient Boosting       | 0.22         | 0.83             | 0.23        | 0.81            |



# Tools & Technologies

- Python 3.x
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (Linear Regression, DecisionTreeRegressor, RandomForestRegressor, GradientBoostingRegressor)
- GridSearchCV for Hyperparameter Tuning



# Visualizations

* Heatmaps for feature correlation
* Time-based ride patterns (rush hours, weekdays)
* Geospatial pickup/drop-off distributions
* Residual plots and prediction-vs-actual graphs

---

# How to Run the Project
 
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/cab-fare-prediction.git
