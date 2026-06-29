# Vendor Invoice Intelligence System

A machine learning-based invoice intelligence system for **freight cost prediction** and **invoice risk detection** using vendor invoice and purchase-order data.

---

## Overview

The Vendor Invoice Intelligence System is designed to analyze vendor invoice and purchase-order records to improve operational efficiency through predictive analytics and anomaly detection.

The system consists of two major modules:

* **Freight Cost Prediction**
* **Invoice Risk Detection**

It uses machine learning models to estimate freight costs and identify suspicious invoices based on engineered business and statistical features.

---

## Features

* Freight cost prediction using regression models
* Invoice anomaly detection using classification models
* SQL-based data extraction and feature engineering
* Automated risk labeling using business rules
* Model persistence for inference and deployment

---

## Tech Stack

* Python
* SQL
* SQLite
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Joblib

---

## Modules

### Freight Cost Prediction

Predicts freight cost using invoice-related features.

Models Used:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

---

### Invoice Risk Detection

Detects suspicious invoices using classification models.

Features Used:

* Invoice Quantity
* Invoice Dollars
* Freight
* Total Item Quantity
* Total Item Dollars

Model Used:

* Random Forest Classifier
* Hyperparameter tuning using GridSearchCV

---

## Dataset

The project uses vendor invoice and purchase-order records stored in SQLite.

Dataset Size:

* 5500+ invoice records

Key attributes include:

* Invoice Quantity
* Invoice Dollars
* Freight
* Purchase Order Number
* Receiving Delay
* Total Item Quantity
* Total Item Dollars

---

## Project Structure

```text id="u42q9v"
Vendor-Invoice-Intelligence-System/
│
├── data/
│   └── inventory.db
│
├── freight_cost_prediction/
│   ├── data_preprocessing.py
│   ├── modeling_evaluation.py
│   └── train.py
│
├── invoice_flagging/
│   ├── data_preprocessing.py
│   ├── modeling_evaluation.py
│   └── train.py
│
├── models/
│   ├── predict_freight_model.pkl
│   ├── predict_flag_invoice.pkl
│   └── scaler.pkl
│
├── notebooks/
│   ├── Predicting Freight Cost.ipynb
│   └── Invoice Flagging.ipynb
│
└── inference/
```

---

## Results

### Freight Cost Prediction

Trained multiple regression models:

* Linear Regression
* Decision Tree Regression
* Random Forest Regression

Random Forest achieved the best performance.

---

### Invoice Risk Detection

Optimized Random Forest classifier using GridSearchCV:

* 216 hyperparameter combinations
* 1080 model fits

Performance:

* Accuracy improved from **80% to 89%**
* Precision: **96%**
* Recall: **71%**

---

## Future Improvements

* Deploy as a web application
* Real-time anomaly detection
* Interactive analytics dashboard
* Improve recall using advanced ML models

---
