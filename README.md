# ⚙️ Predictive Asset Health: RUL Prediction with Machine Learning

## 📄 Project Overview

This project focuses on predicting the Remaining Useful Life (RUL) of engines using the CMAPSS dataset and machine learning models. Predictive maintenance ensures optimal asset utilization and minimizes operational downtime by forecasting the time until a component needs replacement or repair.

The repository demonstrates the complete lifecycle of a predictive analytics project, including data preprocessing, feature engineering, model training, evaluation, and interpretability.

## 📂 Description

The dataset used is the NASA CMAPSS dataset, which contains multi-variate time-series sensor data for engines undergoing degradation. Each engine runs until failure, providing a rich dataset for RUL prediction. This project leverages an XGBoost regression model optimized with grid search and highlights feature contributions using SHAP analysis.

Context and Use-case
Machine learning offers a solution for dynamic maintenance planning in industrial environments by accurately predicting RUL. Engineers can use these predictions to schedule timely interventions, reducing costs and avoiding unexpected failures.

Key dataset attributes:

Sensors: Time-series data from various sensors.
Cycles: Represents the operational age of the engine.
Engine ID: Identifies unique engines in the dataset.

## 📊 Key Features

- _ Machine Learning Model: An XGBoost regressor, optimized for robust performance.
- _ Hyperparameter Tuning: GridSearchCV for optimal parameter selection.
- _ Feature Importance: SHAP values to identify critical sensor features.
- _ Performance Metrics:
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
Mean Absolute Error (MAE)
R² Score
Visualizations:
SHAP feature importance plot
Predicted vs. Actual RUL scatter plot

## 🛠️ Tools & Technologies

Programming Language: Python
Libraries:
XGBoost: Model development
SHAP: Feature interpretability
Pandas, NumPy: Data manipulation
Matplotlib, Seaborn: Data visualization
Scikit-learn: Metrics and preprocessing
Development Environment: Jupyter Notebook

## 📈 Results

Model Performance

MSE: 240.83
RMSE: 15.52
MAE: 11.72
R² Score: 0.86
Feature Importance
SHAP analysis identified the most significant features for predicting RUL, including specific sensor readings and the engine cycle variable.

## 📂 Repository Structure

Data/: Contains the CMAPSS dataset.
Models/: Saved XGBoost model.
Notebooks/: Jupyter notebooks for analysis and model training.
Requirements.txt: Lists Python dependencies.

## 🚀 Future Work

Explore deep learning models like LSTMs for advanced time-series modeling.
Investigate real-time data processing and prediction systems.
Expand interpretability with comparative analysis of features across multiple engines.

