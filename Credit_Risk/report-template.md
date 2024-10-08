# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.


* Explain what financial information the data was on, and what you needed to predict.


* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).



* Describe the stages of the machine learning process you went through as part of this analysis.
The machine learning process involves the practice of model, fit, predict. First, we need to determine our target of the model, in this case, the loan_status column. We then separate this variable from the feature variables, basically all of the columns left after removing the target column. We use train_test_split to separate the training and test data. 

Once we have our training and test split data, we can initialize our model, in this case, a LogisticRegression model. Once we initialize the model, we can fit our training data to that model. The next step is to make predictions! Having fit our training data to the model, the model can now make predictions based on its learning history. The final step is to evaluate how well the model performed. In this project, a confusion matrix and classification report were utilized.


* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
Methods used:

LogisticRegression: a classification tool that is used to predict the probability that a given input falls into one of two classes, hense the classificiation terminology.

Confusion matrix: a tool that generates a table demonstrating effectiveness of the classification model. This tool creates an output comparing predicted labels vs actual labels, how well the predicted labels matched the actual labels.

Classification report: a table outlining model metrics for precision (how many positives were actually positives), recall (how many actual positive instances were correctly identified), f1 score (a mean of precision and recall), and support (actual occurences of each class).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
    0 class:
    - Precision: 1.00, correct prediction of 0 class 100% of opportunities
    - Recall: 0.99, of all class 0 possibilities, model identified 99% of them

    1 class:
    - Precision: 0.84, 84% accuracy predicting the 1 class
    - Recall: 0.94, 94% of all class 1 possibilities were identified by the model

    Overall Accuracy: 99%, model is correct 99% of the time across all overall predictions
    

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The logisitcal model bere performs very well. Both 0 and 1 class performance is important to the overall integrity of the model. It's purpose was to accurately classify the credit worthiness of borrowers, meaning it would have to accurately classify a non-example as a non-example and not a true example, as well as ensure it's labeling true examples as true examples and not true examples as non-examples. This model does that and does that well. I described the results in the question above and both 0 and 1 class precision and recall factors are well above satisfaction.
