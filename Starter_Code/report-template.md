# Module 20 Report Template

## Overview of the Analysis


This analyses used a dataset of historical lending activity to build a model to appraise the healthy loans versus high-risk loans. The dataset shows the loan side, interest rate of the loan, income of borrower, debt versuce income ratio, total debt and loan status. The dataset was clustered by loans status and the results was viewed using the `value_counts` function. 

The stages of the machine learning process are: (a) Instantiate the model, (b) Fit the model, and (c) Use the model.  We run it twice with 1st model in standard logisticRegression and 2nd model in resampling method where we use the RandomOverSampler from the imbalanced-learn library to adjust the data to an equal number of data points.

 

## Results


* Machine Learning Model 1 (Original dataset):
 * The accuracy score is high at 0.99184 or around 99%.
  * The precission is very high for the Healthy Loan which (1) and not that high for High-Risk Loan which is(0.85)
  * The recall for the "0" class is very high (0.99) and high for the "1"class (0.97)



* Machine Learning Model 2:
  * The accuracy score is very higher at 0.99367 or around 99%.
  * The precission is very high for the Healthy Loan which is "0" class(1.00) and lower for High-Risk Loan which is "1" class(0.84)
  * The recall for the Healthy Loan and High-Risk Loan, ("0" and "1")classes matches(0.99)


## Summary

The results show that the accuracy score for the model with oversampled is higher but the precision for the "1" class(High_Risk loan) with oversampled data is lower. And also the recall for the "1" class with the oversampled data is much higher. so that the model that used the oversample data is more accurate at predicting the healthy loan and the risky loan.

As a conclusion using oversampling for this model is not recommended. 
