## 🚀 Bankruptcy Prediction Using Machine Learning
This repository contains a machine learning pipeline for predicting bankruptcy of companies using financial data. The project was developed as part of:

CCAI-312 Pattern Recognition
College of Computer Science and Engineering
University of Jeddah, KSA
Fall Semester 2024

## 📊 Problem Statement
Predict whether a company is alive or bankrupt using financial indicators to help investors, policymakers, and analysts identify early warning signs of financial distress.

## 🗂 Dataset
Source: Kaggle – American Bankruptcy Data

Records: 76,682 companies

Features: 20 financial variables, e.g.:

Current assets

Net income

Total liabilities

Market value

Earnings before interest & tax (EBIT)

Target: status_label → “alive” or “bankrupt”

Class Distribution
Alive → 74,462

Bankrupt → 5,220

Note: The data is highly imbalanced, requiring special handling to avoid biased predictions.

## ⚙️ Machine Learning Pipeline
Preprocessing
Data cleaning and transformation

Class balancing:

Reduced the “alive” class from 74,462 → 35,000 to improve balance

Feature exploration:

Correlation matrix

Histograms

Scatter plots

Algorithms Tested
Algorithm	AUC (All Data)	AUC (Reduced Data)	Remarks
Random Forest	0.87	0.87	Best performance overall
K-Nearest Neighbors	0.72	0.72	Good, but lower recall
Decision Tree	0.64	0.64	Moderate, lower precision
SVC (Support Vector Classifier)	0.68	0.68	Moderate, sensitive to imbalance
Gaussian Naive Bayes	0.58	0.58	Poor for this data
Bernoulli Naive Bayes	0.56	0.56	Poor for imbalanced data
Logistic Regression	Evaluated	Evaluated	Lower than Random Forest

Evaluation Metrics
Accuracy

Precision, Recall, F1-score

Confusion Matrix

ROC Curve

Precision-Recall Curve (PR Curve)

Best Overall Model: Random Forest achieved the highest AUC (0.87) and strong balance between precision and recall.

## 📈 Results
Random Forest achieved:

AUC: 0.87

Strong precision-recall tradeoff

Robustness to imbalance

Other models showed significant performance drops, particularly with imbalanced data.

## 👥 Authors
This project was developed by:

Jameel Rami Mahjub

Abdulrahman Sami Tibagi

Abdulaziz Nasrallah

