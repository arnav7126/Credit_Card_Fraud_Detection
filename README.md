# Credit Card Fraud Detection System

## Overview

This project is a **Credit Card Fraud Detection System** that leverages **Machine Learning** to classify fraudulent transactions. It implements **Logistic Regression** and **XGBoost** models to detect anomalies in financial data and provides a **Streamlit Dashboard** for threshold optimization and cost analysis.

## Features

- **Supervised learning for fraud detection** using a highly imbalanced dataset
- **Logistic Regression & XGBoost** models for classification
- **Threshold tuning** for better fraud detection
- **Cost-based optimization** to minimize financial losses
- **Interactive Streamlit dashboard** for visualization

## Models Implemented

### 1️. **Logistic Regression**

- Uses **balanced class weights** to counteract class imbalance
- Interpreted using **SHAP values**
- **Confusion matrix** analysis

### 2️. **XGBoost Classifier**

- Uses **scale_pos_weight=100** for imbalance handling
- **Hyperparameter tuning** for improved accuracy

## Performance Metrics

| Metric        | Formula               | Description                                   |
| ------------- | --------------------- | --------------------------------------------- |
| **Precision** | TP / (TP + FP)        | % of detected frauds that are actually frauds |
| **Recall**    | TP / (TP + FN)        | % of fraud cases correctly identified         |
| **F1 Score**  | 2 _ (P _ R) / (P + R) | Balance between precision & recall            |
| **AUC-ROC**   | -                     | Measures model discrimination ability         |
| **AUPRC**     | -                     | Precision-recall curve for imbalanced data    |

## Streamlit Dashboard

- **Threshold slider**: Adjusts classification threshold
- **Cost-based analysis**: Calculates fraud cost based on user input
- **Metrics table**: Shows fraud detection performance

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the Streamlit dashboard:
   ```bash
   streamlit run app.py
   ```
