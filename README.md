# Module 20 Report 

## Overview of the Analysis

* The purpose of the analysis is to build a machine learning model that can identify the creditworthiness of borrowers.
* The financial information is on historical lending activity from a peer-to-peer lending services company to predict potential risks in lending or predicting defaults.
* The "loan_status" column provides binary information about the health of the loan: 0 means healthy, and 1 means high risk of defaulting. The distribution of these metrics are as follows: 0 = 75,036 and 1 = 2,500 implying that the vast majority of the loans are healthy.
* The stages of the machine learning process that are part of this analysis include: data collection via the "lending_data" csv file, analyzing the data to understand patters and distributions such as the health of the loan, the use of a logistic regression model as we want to predict as to whether or not a loan is likely to default, train and evaluate the logistic regression model's performance to make predictions for a final evaluation. 
* The algorithms being used are: 'train_test_split' to split the data into training and testing datasets, `LogisticRegression` to predict  a binary outcome (Yes the loan is likely to default, or No the loan is not likely to default), ‘confusion_matrix’ and ‘classification_report’ to evaluate the logistic regression model’s performance.

## Results

* Machine Learning Model: Logistic Regression
*Accuracy score: the ratio of correctly predicted instances to the total instances is 0.99 (99%).
*Precision score: the proportion of true positive predictions in relation to all positive predictions for class 0 is 1.00 (100% precision), and for class 1 is 0.84 (84% precision) means that 84% of the predicted positives were actually positive.
*Recall score: the proportion of true positives that were correctly identified by the model is 0.99 (99%) for class 0 which means the model correctly identified 99% of actual negatives. For class 1: 0.94 (94%) means the model correctly identified 94% of actual positives.

## Summary

Overall, the model performs very well for class 0 (healthy loans), but has room for improvement in predicting class 1 (high risk of defaulting). To improve precision for class 1, we might consider resampling the dataset, tuning the model parameters, and the use of different algorithms to be able to a make a better decision at choosing the right machine learning model. Although there is room for improvements predicting class 1, the overall score of the model is acceptable and should therefore be used.   

