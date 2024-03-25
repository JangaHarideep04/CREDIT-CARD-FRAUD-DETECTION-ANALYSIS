# CREDIT-CARD-FRAUD-DETECTION-ANALYSIS


Credit Card Fraud Detection
Introduction
Credit card fraud is a significant concern for both financial institutions and cardholders. Detecting fraudulent transactions promptly is crucial to minimize financial losses and maintain trust in the banking system. In this project, we aim to develop a machine learning model capable of accurately identifying fraudulent transactions in a dataset of credit card transactions.

Dataset Description
The dataset comprises transactions made by European credit cardholders in September 2013. It includes transactions that occurred over two days, with a total of 284,807 transactions. Among these, there are only 492 instances of fraud, making the dataset highly imbalanced. The positive class (fraudulent transactions) accounts for only 0.172% of all transactions.

Features
Principal Components (V1-V28): These are numerical input variables resulting from a Principal Component Analysis (PCA) transformation. Due to confidentiality reasons, the original features and background information are not provided.
Time: This feature represents the elapsed time in seconds between each transaction and the first transaction in the dataset.
Amount: The transaction amount.
Class: The response variable indicating whether a transaction is fraudulent (Class 1) or not (Class 0).
Project Objective
The primary goal of this project is to build a robust machine learning model capable of accurately detecting fraudulent credit card transactions. Given the highly imbalanced nature of the dataset, special attention will be paid to techniques for handling class imbalance. The model's performance will be evaluated based on metrics such as accuracy, precision, recall, and area under the Receiver Operating Characteristic (ROC) curve.

Methodology
Data Preprocessing: Explore the dataset, handle missing values, scale numerical features, and encode categorical variables (if any).
Feature Engineering: Extract additional features or transform existing ones to improve model performance.
Model Development: Build and fine-tune machine learning models, including algorithms like logistic regression, decision trees, random forests, and XGBoost.
Evaluation: Assess model performance using appropriate evaluation metrics and techniques for imbalanced datasets.
Hyperparameter Tuning: Optimize model hyperparameters using techniques such as grid search or randomized search.
Deployment: Deploy the final model into a production environment for real-time fraud detection.
Model Building with Balancing Classes
Random Oversampling
Results for Random Oversampling with StratifiedKFold technique:

XGBoost ROC AUC: 0.9695
XGBoost Threshold: 0.0014
ROC AUC for the test dataset: 96.9%
SMOTE Oversampling
Results for SMOTE Oversampling with StratifiedKFold:

XGBoost ROC AUC: 0.9837
XGBoost Threshold: 0.0006
ROC AUC for the test dataset: 98.4%
ADASYN Oversampling
Results for ADASYN Oversampling with StratifiedKFold:

XGBoost ROC AUC: ROC AUC value here
XGBoost Threshold: Threshold value here
ROC AUC for the test dataset: ROC AUC value here
Overall, XGBoost model with Random Oversampling and StratifiedKFold technique provided the best results.

Hyperparameter Tuning
HPT_XGBoost Regression:

Model Accuracy: 0.9994037791230966
XGBoost ROC AUC: 0.9284470930852287
XGBoost Threshold: 0.29035016894340515
Conclusion
In summary, Logistic Regression with L2 Regularization for StratifiedKFold cross-validation emerged as the best-performing model without oversampling or undersampling techniques. However, among the oversampling methods, XGBoost with Random Oversampling and StratifiedKFold showed the best results, further optimized through hyperparameter tuning.

This README provides an overview of the project, dataset, methodology, and key results. For more detailed information, refer to the project documentation.
