# Vendor Invoice Intelligence System

Machine Learning based system for **freight cost prediction** and **invoice risk detection** using vendor invoice and purchase-order data.

---

## Overview

The Vendor Invoice Intelligence System analyzes vendor invoice and purchase-order records to predict freight costs and identify suspicious invoices using machine learning.

This project includes:

* Data preprocessing and feature engineering
* Exploratory Data Analysis (EDA)
* Freight cost prediction using regression models
* Invoice anomaly detection using classification models

---

## Features

* Freight cost prediction
* Invoice risk detection
* SQL-based feature engineering
* Automated risk labeling
* Model training and evaluation

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

## Machine Learning Models

### Freight Cost Prediction

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

### Invoice Risk Detection

* Random Forest Classifier
* GridSearchCV for hyperparameter tuning

---

## Dataset

The dataset consists of vendor invoice and purchase-order records stored in SQLite.

Features used:

* Invoice Quantity
* Invoice Dollars
* Freight
* Purchase Order Number
* Receiving Delay
* Total Item Quantity
* Total Item Dollars

Dataset Size:

* 5500+ invoice records

---

## Project Structure

```bash
Vendor-Invoice-Intelligence-System/
│
├── data/
│   └── inventory.db
│
├── notebooks/
│   ├── Predicting Freight Cost.ipynb
│   └── Predicting Flag Invoice.ipynb
│
├── freight_cost_prediction/
│   ├── data_preprocessing.py
│   ├── modeling_evaluation.py
│   └── main.py
│
├── invoice_flagging/
│   ├── data_preprocessing.py
│   ├── modeling_evaluation.py
│   └── main.py
│
├── models/
│
└── README.md
```

---

## Results

### Freight Cost Prediction

Trained multiple regression models:

* Linear Regression
* Decision Tree Regression
* Random Forest Regression

Random Forest achieved the best performance.

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
* Improve recall using advanced ML models
* Add dashboard for analytics
* Enable real-time anomaly detection

---

## Author

Harsh
B.Tech Computer Science with Applied Mathematics
IIIT Delhi
