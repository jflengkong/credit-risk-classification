# Module 12 Report 

## Purpose of the Analysis 
The purpose of this analysis was to develop a potential machine learning model for predicting financial outcomes based on a given dataset. The financial information in the dataset was related to credit card risk. The goal was to build a model and determine the ability for the machine to determine is the set of values given were associated with healthy loan or high-risk loan. 

## Data Description
The dataset features included loan size, interest rate, borrower income, debt-to-income percentage ratio, number of accounts, derogatory marks and total debt. The target was the loan status which contained either a "0" or "1" value. A value of 0 in the “loan_status” column meant that the loan was healthy. A value of 1 means that the loan had a high risk of defaulting. 

## Machine Learning Process
The machine learning process involved several stages: 

Data Preprocessing: Note no data was required to be processed as clean dataset was provided by UWA. 
Feature Selection: Separating the data into labels and features. Note that a copy of the dataset was then varied as to not skew the original data. 
Model Selection: A Logistic regression modal was used to train the data as label consisted of binary classification. 
Model Training: Training the selected models on the training dataset, given the random_state = 1 
Model Evaluation: Evaluating the model's performance by generating a confusion matrix 

## Results

The following clasification report for the test model was generated with the following results: 

[recall screenshot here] 

## Summary

**Question:** How well does the logistic regression model predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

**Answer:** It looks like this logistic regression can predict the healthy loan labelswith high precision and recall (99-100%) more effectively than it can predict the high-risk loans (85-91%). But overall it seems as though that the model is likely to perform well in determining healthy loan predictions.  
