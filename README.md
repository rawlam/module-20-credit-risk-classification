# Predicting Credit Risk of Loans

## Overview of the Analysis

Loans are a crucial part of any modern financial system and economy. Loans help put money in the hands of individuals who may want to buy a car or mortgage a new home. They can help new business owners open up competition. Loans can be seen as the life blood of any modern economy. Therefore, understanding loans and a borrowers credit-worthiness is vital in upholding banks and economies. 

This analysis dives into understanding creditworthiness of borrowers, looking at individual's loan size, interest rate, borrowers income, debt to income ratio, number of accounts, risk level, and loan status. The focus of this analysis will be in predicting the loan status of each borrower through machine learning models where "0" is a health loan and "1" is a high-risk loan.

The machine learning models will be trained and tested on historical lending activity from a peer-to-peer lender services company. The data will first be split into two separate datasets, one for training and the other for testing. The first model logistic regression model, will be trained and the training dataset than tested and evaluated in its predictions on the testing dataset. The second model is similar to the first but with one key difference, before training, it will balance out the original data with RandomOverSampler. The original data is outweighed with significantly more health loans to high-risk loans. The remaining steps are exactly the same as the first model.


## Results

* Machine Learning Model 1: Logistic Regression
  * Accuracy: 0.989
  * Precision: 0.84
  * Recall score: 0.98


* Machine Learning Model 2: Logistic Regression with RandomOverSampler
  * Accuracy: 0.995
  * Precision: 0.99
  * Recall score: 1.00


## Summary

The second model, Logistic Regression with RandomOverSampler, out preformed in predicting high-risk, "1" loan status than just the Logistic Regression model. The scores above indicate a 100% (recall score) identification of high-risk loans, of those 99% (precision) were correctly identified. Taking a closer look, of the 18,616, only three were miss identified as healthy loans. Compare these results to the results of the first model, we can conclude, the second model should be used to evaluation the credit-worthiness of future loans. Banks will save money and modern economies will more likely stay healthy. 