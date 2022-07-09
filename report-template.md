# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.

    **The purpose of the analysis is to build a model that can help identify borrowers creditworthiness by using customer features to determine the `loan status`**

* Explain what financial information the data was on, and what you needed to predict.

    **The model was based on customer credit reports. Features include `loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt`. The model uses these features to predict he label that indicated if a loan has a healthy risk level or if it is high-risk.**

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).

    **The data was imbalanced, as can be expected with this type of data. With 7,5036 loans that are current and 2,500 in default status.**
* Describe the stages of the machine learning process you went through as part of this analysis.
    
    * Split the Data into Training and Testing Sets

    * Create a Logistic Regression Model with the Original Data

    * Predict a Logistic Regression Model with Resampled Training Data 

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

    **Initially we ran a LogisticRegression model on the original dataset. Then due to the data imbalance, we utilized RandomOversampler to resample the data and then fit it to the LR model again. The result was more accurate label predictions.**

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * The logistic regression model scores high marks across the board regarding accuracy (95%), precision(100% for healthy and 85% for high-risk), recall (99% for healthy and 91% for high-risk), and f1 ratio (100% and 88% respectively) for both the majority sample size for healthy loans and minority sample size high risk loans.



* Machine Learning Model 2:
  * The linear Regression model scores high on accuracy (99%), high on precision (100% on healthy and 84% on high risk), high on recall (99% on both), and high on f1 (100% andd 91% respectively). It appears to do a good job of predicting both healthy loans and high-risk loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
    * The resampled model has better overal numbers, and the recall is more favorable to predicting borrowers likely to default.

