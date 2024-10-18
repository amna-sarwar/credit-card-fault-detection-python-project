# Credit Card Fault Detection Python Project

# Project Overview
This project aims to build an efficient credit card fraud detection system using various machine learning algorithms. The project focuses on addressing the challenge of detecting fraudulent transactions from a highly imbalanced dataset, where fraudulent transactions make up a very small percentage of the total transactions.

# Motivation
With the rise of online transactions and digital payments, credit card fraud has become a significant threat to the financial industry. Identifying fraudulent transactions accurately is critical to minimizing losses. This project leverages machine learning algorithms to develop an effective fraud detection model.

# Dataset
The dataset used for this project was sourced from the Credit Card Fraud Detection Dataset available on Kaggle. It contains 284,807 transactions, of which 492 are fraudulent. The data consists of numerical features resulting from a Principal Component Analysis (PCA) transformation, with two untransformed features: Time and Amount. The class label is binary, where 1 indicates a fraudulent transaction and 0 indicates a legitimate one.

Source: Kaggle - Credit Card Fraud Detection
# Data Preprocessing
Given the high imbalance in the dataset, where only 0.172% of transactions are fraudulent, standard machine learning models would struggle to identify fraud accurately. The Synthetic Minority Oversampling Technique (SMOTE) was applied to balance the dataset by oversampling the minority class (fraudulent transactions).

# Algorithms Used
To build a robust fraud detection system, the following machine learning algorithms were employed:

Random Forest
XGBoost
LightGBM
These models were selected based on their performance in handling classification problems and their efficiency in terms of accuracy and prediction. The models were trained on both imbalanced and balanced datasets (after applying SMOTE) to compare performance.

# Model Evaluation
The models were evaluated using the following metrics:

Accuracy: Ratio of correct predictions to the total number of predictions.
Precision: Ratio of true positive predictions to the total predicted positives.
Recall (Sensitivity): Ratio of correctly predicted fraud cases to the actual fraud cases.
F1 Score: Harmonic mean of precision and recall, providing a balanced view of both.
Receiver Operating Characteristic (ROC): Measures the trade-off between true positive and false positive rates.
Matthews Correlation Coefficient (MCC): Measures the quality of binary classifications.
# Results
After applying SMOTE, the models performed significantly better on the balanced dataset. The Random Forest and XGBoost algorithms demonstrated the highest performance across evaluation metrics, including Recall, F1 Score, and MCC. Key findings include:

Random Forest: Best overall performance with high recall and precision after balancing.
XGBoost: Comparable results to Random Forest, with high precision and recall.
LightGBM: Performed well but not as consistently as Random Forest or XGBoost.
# Conclusion
This project highlights the effectiveness of machine learning algorithms, particularly Random Forest and XGBoost, in detecting fraudulent credit card transactions. It also underscores the importance of handling imbalanced datasets using techniques such as SMOTE to improve the model's ability to identify fraud accurately.

Future Work
Future improvements could include:

Exploring neural networks and deep learning techniques.
Applying advanced hyperparameter tuning methods like Grid Search and Randomized Search.
Testing alternative balancing techniques like Borderline-SMOTE.
