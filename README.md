# Data Leakage Detection & Prevention Project

## Project Overview
This project focuses on identifying and fixing **Data Leakage**, one of the most common reasons Machine Learning models fail in production. Using a Credit Card Default dataset, I demonstrate how a "perfect" model can actually be a failure, and how to build a reliable one using professional pipelines.

## The Experiment
I compared two different modeling approaches:
1. **The Leaky Model:** Achieved ~99% accuracy by accidentally using "future" information. 
2. **The Robust Model:** Achieved ~81% accuracy using a **Scikit-Learn Pipeline** and proper feature engineering.

## Key Technical Skills Demonstrated
* **Data Cleaning:** Handled multi-header Excel files and mapped shorthand codes to domain-specific features.
* **Feature Engineering:** Identified and removed leaky proxy variables.
* **Pipelines:** Implemented `StandardScaler` within a `Pipeline` to prevent preprocessing leakage.
* **Model Explainability:** Used **Feature Importance** to verify that the model is making decisions based on logical behavioral patterns.

## Results Summary
* **Base Accuracy:** 81% (Reliable for production)
* **Top Predictors:** Recent payment status (`PAY_0`) and Credit Limit.

## Files in this Repo
* `Data_Leakage_Project.ipynb`: The complete Python notebook with EDA and modeling.
* `default_of_credit_card_clients.csv`: The raw dataset.
