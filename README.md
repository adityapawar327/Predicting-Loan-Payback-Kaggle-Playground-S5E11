# Predicting Loan Payback — Kaggle Playground S5E11

**Author:** Aditya Pawar  
**Competition:** [Kaggle Playground Series S5E11](https://www.kaggle.com/code/adityapawar327/predicting-loan-payback-kaggle-playground/edit)

---

## Overview

This project addresses the binary classification challenge of predicting the likelihood that a loan will be paid back, as posed in Kaggle’s Playground Series S5E11. The solution leverages modern machine learning, with careful data analysis and advanced model tuning methods.

---

## Project Structure

- **predicting-loan-payback-kaggle-playground.ipynb**: Main notebook containing all steps from data loading to model evaluation/submission

---

## Approach

- **EDA:** Comprehensive exploratory data analysis for feature insights, class balance checks (imbalanced), and checks for missing data (none present).
- **Preprocessing:** Cleaning features, handling data types, and feature engineering as needed.
- **Modeling:**  
  - **Algorithm:** XGBoost classifier  
  - **Hyperparameter Tuning:** Automated using Optuna  
  - **Validation:** Robust cross-validation with Repeated K-Fold  
  - **Metrics:** ROC AUC (competition metric)
- **Model Interpretation:** SHAP values plotted for feature importance.
- **Submission:** Generates predictions and prepares formatted `.csv` for Kaggle submission.

---

## Usage

Open and run all cells in `predicting-loan-payback-kaggle-playground.ipynb` in a Kaggle Notebook environment. Installation cells will handle required dependencies.

---

## File Outputs

- `best_xgb_model.pkl` — Trained XGBoost model (pickled)
- `best_params.json` — Optimal tuned parameters
- `tuning_log.txt` — Optuna optimization log
- `submission.csv` — Submission-ready file for Kaggle
- `shap_summary.png` — SHAP feature importance plot

---

## Results

- **Class Distribution:**  
  - Paid back (1): 79.88%  
  - Not paid back (0): 20.12% (Imbalanced)
- **Validation:** Cross-validated ROC AUC
- **Leaderboard:** (Fill in your latest score here after submitting)

---

## Requirements

- Python 3.x
- Kaggle Notebook or local environment with: `xgboost`, `optuna`, `joblib`, `shap`, `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`

---

## Credits

Developed by Aditya Pawar  
For inquiries, reach out via your [GitHub profile](https://github.com/adityapawar327/Predicting-Loan-Payback-Kaggle-Playground-S5E11)

---
