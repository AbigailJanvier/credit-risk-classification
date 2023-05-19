# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
To use different techniques to determine which model is better at detecting healthy and high risk loans.
* Explain what financial information the data was on, and what you needed to predict.
The financial information was loan information that included loan_size, interest_rate,	borrower_income,	debt_to_income,	num_of_accounts,	derogatory_marks,	total_debt, and	loan_status.  I needed to predict whether the loan was healthy or high-risk.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
Value counts showed the amount of high risk and healthy loans besed on the model's assessment of the loan status prodided in the initial dataframe
* Describe the stages of the machine learning process you went through as part of this analysis.
Collecting Data - reading in the csv file
Preparing Data - making dataframes and separating the labels and features
Choosing a Model - Using the logistic regression and random over sampler models
Training the model - using train test split 
Evaluating - getting the balanced accuracy score, confusion matrix, and classification report. 
Parameter tuning - resample the reaning data
Make predictions - evaluate the classification report to see which model is better.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
logistic regression is used to predict the probability of a binary event occuring. It gets the odds of an event occuring in the presence of more than one variable that can explain the outcome.
random over sampling is randomly selecting examples from the minority class in the data and replacing and adding them to the training dataset. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

- Balanced accuracy score: average recall for each class. 
- Precision: how close the accurate measurements are to each other
- Recall: ability to find all relavent cases in a dataset


* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
      - Precision: 100% for healthy loans meaning the model is able to consistently identify healthy loans and 85% for high risk loans
      - Recall: 99% for healthy and 91% for high risk meaning that the model has high sensitivity
      - Accuracy: 99% meaning that the model is able to correctly identify healthy and high risk loans.


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
      - Precision: 100% for healthy loans meaning the model is able to consistently identify healthy loans and 84% for high risk loans
      - Recall: 99% for healthy and 99% for high risk meaning that the model has high sensitivity
      - Accuracy: 99% meaning that the model is able to correctly identify healthy and high risk loans.
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
The RandomOverSampler model performed the best because it had higher recall and F1 score for high risk loans 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Performance does depend on the problem. 

If you do not recommend any of the models, please justify your reasoning.
