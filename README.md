<div align="center">
    <img src="https://performancecardservice.com/wp-content/uploads/2020/12/header-high-risk-payment-processing.jpg">

  <h1 align="center"> Credit Risk Challenge </h1>

  <p align="center">
    UWA Week 20 Challenge
  </p>
</div>

    
## Table of Contents
1. [Project Overview](#project-overview))
    - [Data Description](#%EF%B8%8Fdata-description)
    - [Repository Summary](#repository-summary)
2. [Analysis](#machine-learning-process)
3. [Summary](#summary)

## 📑Project Overview
The purpose of this analysis was to develop a potential machine learning model for predicting financial outcomes based on a given dataset. The financial information in the dataset was related to credit card risk. The goal was to build a model and determine the ability for the machine to determine is the set of values given were associated with healthy loan or high-risk loan. 

## 🖥️Data Description
The dataset features included loan size, interest rate, borrower income, debt-to-income percentage ratio, number of accounts, derogatory marks and total debt. The target was the loan status which contained either a "0" or "1" value. A value of 0 in the “loan_status” column meant that the loan was healthy. A value of 1 means that the loan had a high risk of defaulting. 

## 📊Repository Summary 
- [`Credit_Risk`](https://github.com/jflengkong/credit-risk-classification/tree/main/Credit_Risk)
      - [lending_data.csv](https://github.com/jflengkong/credit-risk-classification/blob/main/Credit_Risk/lending_data.csv)
      - [credit_risk_classification notebook](https://github.com/jflengkong/credit-risk-classification/blob/main/Credit_Risk/credit_risk_classification.ipynb) 
- [`Images`](https://github.com/jflengkong/credit-risk-classification/tree/main/Images)
      - Screenshots of outputs and results
---------------------------------

<div align='center'> 
    
## Machine Learning Process
The machine learning process involved several stages: 

**1. Data Preprocessing:** Note no data was required to be processed as clean dataset was provided by UWA. Below is the [lending_data.csv](https://github.com/jflengkong/credit-risk-classification/blob/main/Credit_Risk/lending_data.csv) read into a Pandas DataFrame. 

![original_data](https://github.com/jflengkong/credit-risk-classification/blob/main/Images/1.original_data.png) 

**2. Feature Selection:** Separating the data into labels and features. Note that a copy of the dataset was then varied as to not skew the original data. 

**3. Model Selection:** A Logistic regression model was used to train the data as label consisted of binary classification. 

**4. Model Training:** Training the selected models on the training dataset, given the random_state = 1 

![logistic_reg](https://github.com/jflengkong/credit-risk-classification/blob/main/Images/2.logistic_reg.png)

**5. Model Evaluation:** Evaluating the model's performance by generating a confusion matrix 

The following clasification report for the test model was generated with the following results: 

![confusion_matrix](https://github.com/jflengkong/credit-risk-classification/blob/main/Images/3.confusion_matrix.png)

## Summary 

**Question:** How well does the logistic regression model predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

**Answer:** It looks like this logistic regression can predict the healthy loan labels with high precision and recall (99-100%) more effectively than it can predict the high-risk loans (85-91%). 

But overall it seems as though that the model is likely to perform well in determining healthy loan predictions.  

</div>


