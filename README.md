# fraud-prediction-automl
This project explores the use of **AutoML**—specifically [FLAML](https://github.com/microsoft/FLAML) by Microsoft—to build and evaluate a predictive model for identifying fraudulent bank applications. 
The goal is to test feasibility, address extreme class imbalance, and generate quick insights using minimal code.

## Dataset
Bank Account Fraud Dataset Suite (NeurIPS 2022)
https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022
variant: base

## Project Overview

Fraud detection problems are challenging due to:
- Highly **imbalanced datasets**
- The need for **high precision and high recall** (minimizing false negatives)

This project demonstrates how **FLAML AutoML** can help:
- Automatically test and tune multiple models
- Improve performance vs baseline models
- Output model insights like feature importance

## Results:
Baseline Decision Tree: PR-AUC ≈ 0.021
FLAML Best Model: PR-AUC ≈ 0.118
📌 FLAML achieved close to 6x improvement in PR-AUC with minimal tuning, showing strong potential for rapid prototyping on imbalanced datasets.

## Key takeaway: 
While FLAML AutoML offers a fast and lightweight way to evaluate modeling feasibility—especially on imbalanced datasets—it currently supports a limited set of model types out of the box (e.g., LightGBM, XGBoost, Random Forest, Logistic Regression).
Thus, AutoML is powerful for quick iteration and validation, but deeper modeling work often requires expanding beyond the default set of algorithms for optimal performance and customization.
