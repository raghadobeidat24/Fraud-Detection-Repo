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

├── EDA.ipynb # Exploratory Data Analysis
├── Models/ # Model training notebooks
│ ├── Model_LogisticRegression.ipynb
│ ├── Model_RandomForest.ipynb
│ ├── Model_XGBoost_All.ipynb
│ ├── Model_XGBoost_Top15.ipynb
├── Best_Model/ # Final chosen model + scaler
│ ├── fraud_LR_model.joblib
│ ├── amount_scaler.joblib
├── requirements.txt # Dependencies
├── README.md # Project description
└── Fraud_Detection_Presentation.pptx # Summary slides



