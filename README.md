# credit-risk-classification
This is my UT Bootcamp Module 20 Challenge

# Credit-Risk-Classification Report

## Overview of the Analysis

* the purpose of the analysis.
The purpose of this analysis is build a model that can identify the creditworthiness of borrowers by using a dataset of historical lending activity from a peer-to-peer lending services company.

* Explain what financial information the data was on, and what you needed to predict.
In this model, financial information like `loan_size` , `interest_rate` , `borrower_income` , `debt_to_income` , `num_of_accounts` , `derogatory_marks` , `total_debt` are trained as features data columns and `loan_status` is our target labels. After fitting in all these training data into the logistics model, some test features data will be needed to fit into the logistic model again to get the predict results.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The variable we are trying to predict is the value counts of `0` (healthy loan) and `1` (high-risk loan). 

* Describe the stages of the machine learning process you went through as part of this analysis.
  * Stage_1: Review that original data and analyse the structure of it.
  * Stage_2: Sperate the label column and the features columns
  * Stage_3: Check the balance fo the lables variable
  * Stage_4: Split the data into training and testing datasets
  * Stage_5: Create a model and fit in the training data
  * Stage_6: Fit in the test data and make prediction
  * Stage_7: Evaluate the model's performance

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
In this analysis, Logistic Regression is usd as the learning and prediction model, and Random Over Sampler is used as an resampled method.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1 (with original train data):
  * Accuracy of Model 1 is 99%;
  * Precision scores for `0`(healthy loan) is 100% and for `1`(high-risk loan) is 87%. 
  * Recall scores for `0`(healthy loan) is 100% and for `1`(high-risk loan) is 89%.



* Machine Learning Model 2 (with random over sample train data):
  * Accuracy of Model 1 is 100%;
  * Precision scores for `0`(healthy loan) is 100% and for `1`(high-risk loan) is 87%. 
  * Recall scores for `0`(healthy loan) is 100% and for `1`(high-risk loan) is 100%.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Comparing the results, we can conclude that Machine Learning Model 2 (with random over sample train data) seems preform better, because the accuracy score is higher.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Yes, the performance depends on the problem we are trying to solve. It is more important to predict the `1`'s to identify the high risk loan. In Model 2, we have an accuracy of 100% and recall score of 100% for `1`'s, which means the model could predict the target very well.

If you do not recommend any of the models, please justify your reasoning.
According to the results, we recommend this model.