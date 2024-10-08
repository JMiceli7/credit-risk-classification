# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis is to build and evaluate a machine learning model that will accurately classify the creditworthiness of a borrow. They would need to be able to classified as not creditworthy, or creditworthy.

The dataset featured historical lending data from a peer to peer lending service. It included loan size, interest rate, borrow income, debt to income, number of accounts, derogitory remarks, and total debt. This model needed to be able to predict accurate classifications of loan status based on these features. Thus, loan status is the variable we are trying to accurate predict. 

The machine learning process involves the practice of model, fit, predict. First, we need to determine our target of the model, in this case, the loan_status column. We then separate this variable from the feature variables, basically all of the columns left after removing the target column. We use train_test_split to separate the training and test data. 

Once we have our training and test split data, we can initialize our model, in this case, a LogisticRegression model. Once we initialize the model, we can fit our training data to that model. The next step is to make predictions! Having fit our training data to the model, the model can now make predictions based on its learning history. The final step is to evaluate how well the model performed. In this project, a confusion matrix and classification report were utilized.

## Methods used:

LogisticRegression: a classification tool that is used to predict the probability that a given input falls into one of two classes, hense the classificiation terminology.

Confusion matrix: a tool that generates a table demonstrating effectiveness of the classification model. This tool creates an output comparing predicted labels vs actual labels, how well the predicted labels matched the actual labels.

Classification report: a table outlining model metrics for precision (how many positives were actually positives), recall (how many actual positive instances were correctly identified), f1 score (a mean of precision and recall), and support (actual occurences of each class).

## Results

* Machine Learning Logistical Regression (classification model):
    * Description of Accuracy, Precision, and Recall scores:
      0 class:
      - Precision: 1.00, correct prediction of 0 class 100% of opportunities
      - Recall: 0.99, of all class 0 possibilities, model identified 99% of them

      1 class:
      - Precision: 0.84, 84% accuracy predicting the 1 class
      - Recall: 0.94, 94% of all class 1 possibilities were identified by the model

    Overall Accuracy: 99%, model is correct 99% of the time across all overall predictions
    

## Summary

The logisitcal model bere performs very well. Both 0 and 1 class performance is important to the overall integrity of the model. It's purpose was to accurately classify the creditworthiness of borrowers, meaning it would have to accurately classify a non-example as a non-example and not a true example, as well as ensure it's labeling true examples as true examples and not true examples as non-examples. This model does that and does that well. I described the results in the question above and both 0 and 1 class precision and recall factors are well above satisfaction and definitely the recommended tool for the job.
