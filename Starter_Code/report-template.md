# Module 12 Report Template

## Credit Risk Analysis Report ##

## Overview of the Analysis

In the current analysis, we create and utilize a Supervised Machine Learning Model for the processing of Crypto-Currency data. This Crypto currency contains data columns loan loan_size,interest_rate,borrower_income,debt_to_income,num_of_accounts,derogatory_marks,total_debt,loan_status. Our aim is to be able to use this model to predict whether an instance would likely be a healthy loan [Class 0] or high-risk loan [Class 1]. Our primary variables of interest included: 
    
    a. loan_size
    b. interest_rate
    c. borrower_income
    d. debt_to_income
    e. num_of_accounts
    f. derogatory_marks
    g. total_debt
    h. loan_status

    Our model aims to utilize these parameters to predict whether an incoming account would tend towards being a healthy loan or a high-risk loan. 

    The data file supplied is in CSV format. 

    Our model's machine learning process are as described below: 
    a. Data splitting into Training and Testing Sets 
    --> Read data split into labels and features, with the labels referring to the loan type (healthy vs. high-risk) and all other columns/variables as the features 
    --> Data sets were 'split,' or separated into training versus testing datasets 

    b. Creation of a Logistic Regression Model with the
    Original Data 
    --> Using the Sklearn package, we were able to create a Logistic Regression model
    --> Binary Classifier ([0] vs [1] were the viable predictions)
    --> Fitting of this model was completed by using the training data 
    --> Predictions were made using this model by supplying the testing data

    c. Evaluation and Summarization of the findings

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model Accuracy, Precision, and Recall scores.

    *Accuracy: 0.99 (weighted average) indicates a correct prediction 99% of the times it makes a prediction using the given parameters 

    *Precision:
    [0] Healthy Loan: 1.00
    [1] High-Risk Loan: 0.85

    *Recall:
    [0] Healthy Loan: 0.99
    [1] High-Risk Loan: 0.91

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.


# CryptoClustering Assignment 

Write a Credit Risk Analysis Report (20 points)
To receive all points, you must:
•	Provide an overview that explains the purpose of this analysis. (5 points)
•	Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)
•	Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

## Credit Risk Analysis Report ##


### Analysis Overview ###

### Machine Learning Model Review: Results ###

### Results Summary ###
