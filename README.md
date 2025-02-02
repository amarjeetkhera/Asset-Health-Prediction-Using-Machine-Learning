# ⚙️ Asset Health Prediction Using Machine Learning

## 📄 Project Overview

This project focuses on predicting the Remaining Useful Life (RUL) of engines using the CMAPSS dataset and machine learning models. Predictive maintenance ensures optimal asset utilization and minimizes operational downtime by forecasting the time until a component needs replacement or repair.

The repository demonstrates the complete lifecycle of a predictive analytics project, including data preprocessing, feature engineering, model training, evaluation, and interpretability.

## 📂 Description

Machine learning offers a solution for dynamic maintenance planning in industrial environments by accurately predicting RUL. Engineers can use these predictions to schedule timely interventions, reducing costs and avoiding unexpected failures.
The dataset used is the NASA CMAPSS dataset contains multi-variate time-series sensor data for engines undergoing degradation. Each engine runs until failure, providing a rich dataset for RUL prediction. Each dataset in the Data folder is a separate time series adhering to different fault types. For this project, only the FD001 data has been taken into consideration.


Key dataset attributes:

Sensors: Time-series data from various sensors.

Cycles: Represents the operational age of the engine.

Engine ID: Identifies unique engines in the dataset.

## 📊 Key Features

- Machine Learning Model: An XGBoost regressor, optimized for robust performance.
- Hyperparameter Tuning: GridSearchCV for optimal parameter selection.
- Feature Importance: SHAP values to identify critical sensor features.
- Performance Metrics:
    - Mean Squared Error (MSE)
    - Root Mean Squared Error (RMSE)
    - Mean Absolute Error (MAE)
    - R² Score

## 🛠️ Tools & Technologies

- Programming Language: Python
  
- Development Environment: Jupyter Notebook

## 📈 Results

- MSE: 247.66
  
- RMSE: 15.73

- MAE: 12.09
  
- R² Score: 0.85

## 📂 Repository Structure

- Data/: Contains the CMAPSS dataset.
  
- Models/: Saved XGBoost model.

- Notebooks/: Jupyter notebooks for analysis and model training.

## 🚀 Future Work

- Although it can be computionally expensive, deep learning models like LSTMs can be explored with higher number of time-steps for capturing long-term dependencies in the data. In this project an implemention of LSTM has been covered with timestep = 1 for simplicity yielding a model which underperforms.
  
- Real-time data processing and prediction systems can be investigated with extended visualization of the KPIs through a web app for real time usage.
  
- Expand interpretability with comparative analysis of features across multiple engines.

- More engineered features can be explored.

