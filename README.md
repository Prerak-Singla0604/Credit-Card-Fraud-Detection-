

# 💳 Credit Card Fraud Detection
This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The dataset used for this project is sourced from Kaggle and contains anonymized features due to confidentiality concerns. The goal of the project is to build a model that accurately predicts whether a given transaction is fraudulent or genuine based on the provided numerical parameters.

## 🚧 Project Overview
The goal is to develop a model that accurately predicts whether a transaction is fraudulent or legitimate based on several anonymized features from the dataset.

## 📈 Dataset Overview
The dataset consists of transactions made by European credit cardholders in September 2013. It contains 284,807 transactions, of which 492 are labeled as frauds, creating a highly imbalanced dataset where fraud accounts for only 0.172% of all transactions. All input features are numerical, transformed through Principal Component Analysis (PCA) to ensure privacy. The dataset includes the following notable features:
- **Time**: Seconds elapsed between each transaction and the first transaction in the dataset.
- **Amount**: Transaction amount, which can be used for cost-sensitive learning.
- **Class**: The target variable, where 1 indicates a fraudulent transaction, and 0 indicates a genuine transaction.

Given the class imbalance, traditional accuracy metrics may not be meaningful. Instead, the Area Under the Precision-Recall Curve (AUPRC) and Receiver Operating Characteristic (ROC) curve are more appropriate to evaluate model performance.


- **Dataset Link:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- 
### Logistic Regression
Logistic regression is used in this project to model the probability of a transaction being fraudulent. This algorithm is effective for binary classification problems like fraud detection. In this project, we enhanced the logistic regression model by using the **Receiver Operating Characteristic (ROC) curve** to identify the optimal decision threshold. This threshold was then used in the logistic regression model to achieve better accuracy in predicting frauds.

By analyzing the ROC curve, we optimized the trade-off between sensitivity and specificity to maximize the detection rate for fraudulent transactions while minimizing false positives.

![logistic-regression-example](https://user-images.githubusercontent.com/56130865/163219252-a8caf755-3eb7-47d4-be12-3767d75ebe12.jpg)
