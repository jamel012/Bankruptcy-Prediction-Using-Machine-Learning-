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
Below is our end-to-end pipeline for this project:
<img width="360" height="859" alt="image" src="https://github.com/user-attachments/assets/4595b466-be2d-470b-bd42-1d667d6fe335" />
## 🔎 Data Exploration

We explored feature relationships using a correlation heatmap:

<img width="612" height="597" alt="image" src="https://github.com/user-attachments/assets/4c06f6d6-aa83-4591-8454-b7ae93333b7c" />

We also visualized feature relationships with scatter plots:

<img width="624" height="605" alt="image" src="https://github.com/user-attachments/assets/473084c7-685c-453d-bbb2-4f2a0fcf1edc" />


## 📊 Model Evaluation and Results

Here’s our comparison of algorithms:

<img width="633" height="426" alt="image" src="https://github.com/user-attachments/assets/fc93a1ef-aa8c-4bd6-9006-908dc74d0a74" />

### Precision-Recall Curve

Random Forest achieved the best PR AUC:

<img width="1055" height="420" alt="image" src="https://github.com/user-attachments/assets/f9d37aa5-78b6-46ca-bcb3-7263e211ecab" />

### ROC Curve

ROC comparison across models:

<img width="900" height="420" alt="image" src="https://github.com/user-attachments/assets/a47f7010-ae66-49d8-a834-60e916aa214f" />


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

