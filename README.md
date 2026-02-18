# 🚗 Car Price Prediction using KNN Regression

## 📌 Overview
This project predicts car prices using the K-Nearest Neighbors (KNN) Regressor.

The goal is to understand how distance-based algorithms perform in regression tasks and how preprocessing techniques affect model performance.

---

## 📊 Dataset
Automobile Dataset (UCI Machine Learning Repository)

Target Variable:
- price

---

## 🛠 Project Workflow

1. Data Cleaning
   - Replaced '?' with NaN
   - Converted numeric columns
   - Handled missing values
   - Removed zero-variance features

2. Outlier Handling
   - Applied IQR method
   - Reduced noise and improved RMSE

3. Encoding
   - Label Encoding for binary features
   - One-Hot Encoding for multi-class features

4. Feature Scaling
   - StandardScaler applied to all features
   - Critical for KNN performance

5. Model Training
   - KNN Regressor
   - Manhattan distance
   - Distance weighting

6. Hyperparameter Tuning
   - Tested K values from 1 to 30
   - Selected optimal K based on RMSE

---

## 📈 Model Performance

- MAE: 1101
- RMSE: 1514
- R² Score: 0.85

---

## 📊 Visualization

- RMSE vs K plot
- Actual vs Predicted prices plot

The model demonstrates strong predictive performance with good generalization.

---

## 💡 Key Insights

- Scaling is essential for distance-based models.
- Removing outliers significantly improved RMSE.
- KNN tends to smooth extreme values due to averaging behavior.
- Manhattan distance performed better than Euclidean for this dataset.