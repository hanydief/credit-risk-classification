# credit-risk-classification
Use various techniques to train and evaluate a model based on loan risk. Use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

## Classmate Contributors on study group: 
Thank you for helping on Challenge Study Group:
- Vinny Shankar -- [Vinny Shankar](https://github.com/VinnyShankar)
- Jesús Jiménez -- [Jesús Jiménez](https://github.com/JesusJimenez3318)


## Split the Data into Training and Testing Sets (30 points)
To receive all points, you must:

- Read the lending_data.csv data from the Resources folder into a Pandas DataFrame. (5 points)

- Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns. (10 points)

- Split the data into training and testing datasets by using train_test_split. (15 points)

![P1-SplitData]()

## Create a Logistic Regression Model (30 points)
To receive all points, you must:

- Fit a logistic regression model by using the training data (X_train and y_train). (10 points)

- Save the predictions on the testing data labels by using the testing feature data (X_test) and the fitted model. (5 points)

- Evaluate the model’s performance by doing the following:

  - Generate a confusion matrix. (5 points)

  - Generate a classification report. (5 points)

  - Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels? (5 points)

![P2-Logistic-Regression_Original-data]()
![P3-Logistic-Regression_Resampled_data]()

# Write a Credit Risk Analysis Report (20 points)
To receive all points, you must:

- Provide an overview that explains the purpose of this analysis. (5 points)

- Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model. (5 points)

- Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning. (10 points)

## Summary

Analysis show that collected data can be effectively used to train and test the Machine Learning Classification Model. For better preditions solving the imbalance sampling issue is needed.

Randomly oversampling the data helps us to get higher balanced accuracy and recall scores. With higher recall value, model can predict risky loans more accurately.

With incorrect predictions we have two issues:

    False positives (where users are flagged as risky, but are actually healthy)
    False negatives (where users are not flagged as risky but are actually risky)

both cases have its costs. It is important to predict both 1s and 0s. Therefore, model should have good accuracy in terms of both.

# Coding Conventions and Formatting (10 points)
To receive all points, you must:

- Place imports at the top of the file, just after any module comments and docstrings and before module globals and constants. (3 points)

- Name functions and variables with lowercase characters, with words separated by underscores. (2 points)

- Follow DRY (Don’t Repeat Yourself) principles, creating maintainable and reusable code. (3 points)

- Use concise logic and creative engineering where possible. (2 points)

Code Comments (10 points)
To receive all points, your code must:

- Be well commented with concise, relevant notes that other developers can understand. (10 points)
