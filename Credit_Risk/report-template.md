# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  - Description of Model 1 Accuracy, Precision, and Recall scores.
  - Accuracy score: 99%- good!
  - Healthy loans see ideal precision and f1 scores at 100%, while recall is at 99%
  - High-risk loans' precision is 15% lower than healthy loans
  - High-risk loans are also at lower recall and f1-score values than the healthy loans with 8% and 2% variations (respectively)



* Machine Learning Model 2:
  - Description of Model 2 Accuracy, Precision, and Recall scores.
  -  Accuracy score: 99%- good!
  -  Precison, recall, and f1 have remained the same for healthy loans
  -  High-risk loans experienced general increase in recall and f1-score- 8% and 3% (respectively)
  -  High-risk loans experienced a decrease in precision by 1%


## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
both they are so close, but Model 2 looks more accurate with 0.95 compared to 0.94 macro average but both accuracy are 0.99
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

It is important to predict both the ones and zeros in order to determine a the creditworthiness of borrowers. Being able to compare the two allows for well-rounded predictions and conclusions to be made.

ALSO,

Analysis show that collected data can be effectively used to train and test the Machine Learning Classification Model. For better preditions solving the imbalance sampling issue is needed.

Randomly oversampling the data helps us to get higher balanced accuracy and recall scores. With higher recall value, model can predict risky loans more accurately.

With incorrect predictions we have two issues:

    False positives (where users are flagged as risky, but are actually healthy)
    False negatives (where users are not flagged as risky but are actually risky)

both cases have its costs. It is important to predict both 1s and 0s. Therefore, model should have good accuracy in terms of both.