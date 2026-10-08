# Machine Learning Assignment 1 — Polynomial Regression

**Roll Number:** BT2024129

This repository contains the implementation and results for Machine Learning Assignment 1, covering two personalized polynomial regression problems: VAR 1 and VAR 2.

## Contents

- `VAR1_Polynomial_Regression.ipynb` — Polynomial regression implementation for VAR 1
- `VAR2_Polynomial_Regression.ipynb` — Polynomial regression implementation for VAR 2
- `BT2024129_pred_var1.csv` — Final predictions for VAR 1
- `BT2024129_pred_var2.csv` — Final predictions for VAR 2
- `BT2024129_ML_Assignment_1_Report.pdf` — Assignment report

## Methodology

The models use polynomial feature expansion, feature scaling, and regularized regression. Five-fold shuffled cross-validation with `random_state=42` and `GridSearchCV` was used for model selection. Mean Squared Error (MSE) was used as the primary validation metric.

### VAR 1

- Features: 6
- Final model: **Lasso Regression**
- Polynomial degree: **5**
- Alpha: **0.01389495494**
- Cross-validation MSE: **0.3381889241**
- Training R²: **0.97295**

### VAR 2

- Features: 3
- Final model: **Lasso Regression**
- Polynomial degree: **10**
- Alpha: **0.000316227766**
- Cross-validation MSE: **0.2531166843**
- Training R²: **0.996510**

An additional Elastic Net experiment was performed for VAR 2, but it was not used for the final predictions.

## Final Model Summary

| Problem | Model | Degree | CV MSE |
|---|---|---:|---:|
| VAR 1 | Lasso | 5 | 0.338189 |
| VAR 2 | Lasso | 10 | 0.253117 |

## Libraries Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook
- Matplotlib

## Author

**BT2024129**

## GitHub Repository

https://github.com/muzhaib/BT2024129-ML-Assignment-1
