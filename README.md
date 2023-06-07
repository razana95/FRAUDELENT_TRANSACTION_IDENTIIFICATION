# FRAUDELENT_TRANSACTION_IDENTIIFICATION

This repository contains the code and documentation for the Fraudulent Transaction Identification project. The project aims to develop a classification model that can accurately identify fraudulent transactions. By leveraging machine learning techniques and data analysis, the model can assist in mitigating fraud risks and protecting financial systems.

## Table of Contents

Project Overview
Dataset
Installation
Usage
Results
Contributing

## Project Overview

The Fraudulent Transaction Identification project involves several steps to build an effective model for fraud detection. The key steps include data cleaning, feature engineering, fraud trends analysis, model training, variable selection, and performance evaluation. By following these steps, the project aims to achieve accurate predictions of fraudulent activities.

## Dataset

The dataset used for this project contains various features related to transactions, such as transaction amounts, timestamps, and transaction types. The dataset is obtained from https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset

## Installation

To run the code and reproduce the results, follow these steps:

Clone this repository
Install the required dependencies:
Download the dataset from [https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset] and place it in the data directory.

## Usage

Follow these steps to use the Fraudulent Transaction Identification system:

### 1)Data Cleaning:
Analyzed the dataset using info() and describe() to understand its characteristics.
Checked for missing values and determined that no treatment was required.
Verified and removed duplicates from the dataset.
Handled outliers by identifying extreme values and retaining them as valid and important for the model.
### 2)Feature Engineering:
Created new columns based on the existing features to enhance the predictive power of the model.
Converted the step column into corresponding hour, day, month, and year columns.
Removed the year and month columns due to limited variation.
Examined fraud trends by analyzing the day, hour, and isFraud columns.
Calculated the balance difference after transactions for both senders and receivers.
Detected and encoded anomalies in the data.
Applied feature scaling using the Robust Scaler to handle outliers.
### 3)Fraud Detection Model:
Trained a logistic regression model to detect fraudulent transactions.
Addressed the highly imbalanced dataset using SMOTE and RandomUnderSampler techniques.
Utilized the Decision Tree algorithm, fine-tuned it using RandomizedSearchCV, and performed cross-validation.
Evaluated the model's performance using various metrics such as ROC-AUC, recall, confusion matrix, and classification report.
### 4)Variable Selection:
Selected relevant variables based on domain knowledge and exploratory data analysis.
Identified key variables related to time, transaction balances, transaction types, and derived variables capturing changes in balances.
### 5)Performance Demonstration:
Assessed the model's performance using evaluation metrics and cross-validation results.
Achieved an ROC-AUC score of 94% and recall of 0.93 after addressing the class imbalance.
### 6)Fine Tuning and Performance Evaluation:
Fine-tuned the model using RandomizedSearchCV and performed cross-validation for further improvement.
Key Factors Predicting Fraudulent Customers:
Identified the importance of transaction balances, transaction types, and temporal patterns in predicting fraudulent transactions.
Highlighted the alignment of these factors with known fraud patterns.
### 7)Interpretation of Factors:
Interpreted the identified factors and their alignment with common characteristics associated with fraudulent behavior.
Noted the significance of abnormal transaction balances, specific transaction types, and unusual temporal patterns in detecting fraud.
### 8)Prevention Strategies:
Suggested prevention strategies to mitigate fraud risks, including enhanced authentication protocols, real-time monitoring systems, and anomaly detection algorithms.
Emphasized the importance of continuously updating and improving the infrastructure to stay ahead of evolving fraud patterns.
### 9)Evaluation of Prevention Actions:
Proposed evaluating the effectiveness of prevention actions through ongoing monitoring, continuous improvement, and regular assessment of fraud detection and prevention measures.
Recommended using evaluation metrics, monitoring systems, and benchmarks to measure the impact of prevention measures accurately.


## Results

The Fraudulent Transaction Identification project aims to achieve accurate predictions of fraudulent transactions. The results of the model can be summarized as follows:

Achieved an ROC-AUC score of 94% and recall of 93%.
Successfully identified key factors related to transaction balances, transaction types, and temporal patterns that are indicative of fraudulent activities.
Provided prevention strategies, including enhanced authentication protocols, real-time monitoring systems, and anomaly detection algorithms, to mitigate fraud risks.
Emphasized the importance of continuous improvement, monitoring, and evaluation of fraud prevention measures.

## Contributing

Contributions to this project are welcome. If you have any suggestions, improvements, or new ideas, please feel free to open an issue or submit a pull request.







