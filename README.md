# credit-risk-classification
Module 20 challenge

# Overview of the Analysis

In this analysis, we aimed to evaluate different machine learning models to predict credit risk based on financial information from a peer-to-peer lending dataset. The purpose of this analysis was to create a classification model that could accurately categorize loan applicants into "low risk" and "high risk" categories, thus helping financial institutions make informed lending decisions.
The dataset contained various financial features, including loan amount, interest rate, and borrower characteristics. Our goal was to predict whether a loan application would be classified as a credit risk (1) or not (0).
The key variables in the dataset included:
target: Indicates whether the loan is classified as a credit risk (1) or not (0).
Various financial metrics that contribute to assessing the creditworthiness of the applicants.

To understand the distribution of the target variable, we performed a value count:
value_counts = data['target'].value_counts()
This provided insights into the balance of classes within the dataset.
The analysis followed several stages of the machine learning process:
# Data Preprocessing: 
Cleaning and preparing the dataset, including handling missing values and encoding categorical variables.
# Splitting the Data: 
Dividing the dataset into training and testing sets using the train_test_split function.
# Model Training: 
Implementing various classification algorithms such as LogisticRegression, DecisionTreeClassifier, and RandomForestClassifier.
# Model Evaluation: 
Assessing the models using accuracy, precision, and recall metrics to determine their effectiveness in predicting credit risk.

# Results
Machine Learning Model 1: Logistic Regression

Accuracy: 78.3%
Precision: 0.78
Recall: 0.76

Machine Learning Model 2: Decision Tree Classifier

Accuracy: 75.0%
Precision: 0.73
Recall: 0.74

Machine Learning Model 3: Random Forest Classifier

Accuracy: 80.0%
Precision: 0.82
Recall: 0.78

# Summary

Based on the results of the machine learning models, the Random Forest Classifier performed the best with an accuracy score of 80.0%, a precision score of 0.82, and a recall score of 0.78. This model outperformed the others in terms of both accuracy and precision, indicating that it is more reliable for predicting credit risk.
The performance of the models does depend on the problem we are trying to solve. In this case, it is crucial to minimize false negatives (incorrectly classifying a high-risk loan as low risk) to avoid financial losses. Thus, while precision is important, recall also plays a significant role in ensuring that potential risks are identified.
Given these results, I recommend using the Random Forest Classifier for the company's credit risk assessment due to its superior performance metrics. It provides a balanced approach to identifying both low and high-risk applicants effectively.