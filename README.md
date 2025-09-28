# Fraud Detection Case Study – Credit Card Transactions
## Project Overview

The goal of this project is to design a predictive model that detects fraudulent credit card transactions, moving from a reactive to a proactive fraud detection strategy.

Fraud is rare (<1.2% of all transactions) but costly. Our analysis shows it is not random: it clusters around specific merchants, categories, and higher transaction amounts.

## #Key Result:
The models can detect up to 98% of fraud cases, representing ~$13.9M/month in prevented fraud losses.

## Objectives

Analyze a dataset of ~595K credit card transactions.

Understand fraud distribution and patterns through EDA.

Build multiple ML models to classify fraud vs. non-fraud.

Compare performance with metrics suited for imbalance (Recall, Precision, F1, ROC-AUC).

Translate results into business impact (ROI).

## Repository Structure
```
├── EDA.ipynb # Exploratory Data Analysis
├── Models/ # Model training notebooks
│ ├── LogisticRegression.ipynb
│ ├── RandomForest.ipynb
│ ├── XGBoost_All.ipynb
│ ├── XGBoost_Top15.ipynb
├── Best_Model/ # Final chosen model LogReg + scaler
│ ├── fraud_LR_model.joblib
│ ├── amount_scaler.joblib
├── requirements.txt # Dependencies
├── README.md # Project description
└── Fraud_Detection.pptx # Project Power Point slides
```

## Methodology

EDA: Checked imbalance, fraud patterns, transaction amounts, categories, and merchants.

Feature Engineering: Added day, hour, and time_of_day from the step column.

Models: Logistic Regression, Random Forest, XGBoost (all + top 15 features).

Evaluation Metrics: Recall, Precision, F1, ROC-AUC.
## Results (Test Data)

| Model               | Accuracy | Recall | Precision | ROC-AUC |
|----------------------|----------|--------|-----------|---------|
| Logistic Regression  | 97.5%    | 0.98   | 0.32      | 0.997   |
| Random Forest        | 98.1%    | 0.91   | 0.38      | 0.986   |
| XGBoost (All)        | 97.6%    | 0.97   | 0.33      | 0.997   |
| XGBoost (Top 15)     | 96.0%    | 0.97   | 0.22      | 0.995   |




