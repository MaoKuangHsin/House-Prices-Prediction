# 🏡 House Price Prediction using Linear Regression & Feature Engineering

This project explores the predictive power of linear regression models enhanced with custom feature engineering techniques.  
It includes benchmarking against XGBoost and a step-by-step breakdown across five Jupyter notebooks.

---

## 📌 Project Overview

- **Goal**: Predict house prices using interpretable linear models and custom features
- **Dataset**: `house_dataset.csv` with room size, location, and condition attributes
- **Target Variable**: `price` (log-transformed to `log10_price`)
- **Evaluation Metric**: MAPE (Mean Absolute Percentage Error)

---

## 🗂️ Project Structure

- `Step 1.ipynb`: Data cleaning and log transformation
- `Step 2.ipynb`: Exploratory data analysis (EDA)
- `Step 3.ipynb`: Feature engineering (numerical, categorical, KNN)
- `Step 4.ipynb`: Linear model training (OLS, Ridge, Lasso, Elastic Net)
- `Step 5.ipynb`: XGBoost benchmarking and residual analysis

---

## 🛠️ Key Techniques

- Log and squared feature transformations
- Feature interaction terms (e.g., bedrooms × bathrooms)
- Domain-informed ratios (e.g., living area per lot)
- Target encoding for location
- KNN-based pricing context feature
- Model comparison: OLS, Ridge, Lasso, Elastic Net, XGBoost

---

## 📊 Results Summary

| Model        | CV MAPE | Test MAPE |
|--------------|---------|-----------|
| Baseline OLS | 15.7%   | 25.82%    |
| Ridge        | 15.7%   | 25.81%    |
| Lasso        | 15.8%   | 25.83%    |
| Elastic Net  | 15.7%   | 25.75%    |
| XGBoost      | 21.9%   | **18.66%**|

Elastic Net offered a strong balance between accuracy and interpretability.  
XGBoost provided the lowest test MAPE but with increased complexity.

---

## 🔮 Future Directions

- Apply the feature pipeline to other housing datasets
- Add spatial and temporal trends
- Use SHAP values for model explanation
- Explore ensemble stacking with interpretable components




