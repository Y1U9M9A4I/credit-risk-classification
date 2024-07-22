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

Our model does a phenomenal job at predicting [0] Healthy Loans, with a precision of 100% and a recall of 99%. We see a step down in prediction precision to 85% when predicting [1] High-Risk Loans, and a drop in recall to 91%. This model presents promise in prediction of high-risk loans and proven accuracy in predicting healthy loans. 

Considering the weighted average in precision is 99% for the model as a whole, we should be suspicious of unequal datasets potentially contributing to these differences in precision numbers ([0] may have more data for which the algorithm can learn and predict). By calling on additional information for each [0] and [1] through a value_count, we can see that we have much more data for Healthy Loans [0] than High-Risk Loans [1], and this near 30x more data supplied for Healthy Loans may explain the prediction precision difference of this model for either loan statuses.

In a sense of practical application, it would be much more critical to predict High Risk Loans (and proceed with more caution) versus identifying healthy loans. The practical applicability of this model would therefore be in the identification of loans to not approve [high risk loans, [1]]. 

Although the modeling accuracy for prediction of [1] is lower than for [0], it is still a reasonably accurate model. I would recommend the model for usage, but also heavily consider the necessary addition of more high-risk data data sets in order to improve the model for prediction of [1].
