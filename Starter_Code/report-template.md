# Module 12 Report

## Overview of the Analysis


This analysis serves to use machine learning to build a model that can identify the credit worthiness of borrowers based on historical activity from a peer to peer lending service. This historical data included various data that is impactful to the whether or not a lender will grant a requested loan, such as: loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt and whether or not the loan was historically approved.

The machine learning technique used took a deeper dive into value_counts; splitted the data to trained data and test data via train_test_split; used the data to train via logistic regression models; and even resampled the data to balance out imbalanced data (via oversampling) in an effort to understand unapproved loans better.

This analysis extracted the raw data into a format more compatible to the machine learning model, split the data, trained the model to learn the data via logistic regression, and even resampled the data with a "randomoversampler" model, then used the original data to test the effectiveness of the model. At the end various reports were created to check accuracy, precision, recall and f1 scores.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  - Balanced Accuracy 
  The balanced accuracy score for Machine 1 is 95.10%. This score is a very good overall score in whether or not the machine can determine if a loan is a healthy loan or a risky loan based on the features listed in the model. A balanced accuracy score of 95.10% means that the machine can determine true postives (while factoring false negatives) and true negatives (while factoring false positives) around 95% of the time.
  - Precision
  The precision score for Machine 1 is 100% for predicting healthy loans (0) and 86% for predicting risky loans (1). The precision score determines whether or not a machine can predict True Positives while factoring the False Positives. While a 100% chance in predicting precision in healthy loans is excellent, an 86% chance for predicting precision in risky loans is only considered good -- and this would be the focus of the machine for the company.
  - Recall
  The recall score for Machine 1 is 99% for predicrting healthy loans (0) and 91% for predicting risky leans (1). The recall score determines whether or not a machine can predict True Positives while factoring the False Negatives. While a 99% chance in predicting precision in healthy loans is excellent, an 91% chance for predicting precision in risky loans is very good. This score is important to the company but is not the main focus of the company in assessing risky loans.



* Machine Learning Model 2:
   - Balanced Accuracy 
  The balanced accuracy score for Machine 1 is 99.49%. This score is an excellent overall score in whether or not the machine can determine if a loan is a healthy loan or a risky loan based on the features listed in the model. A balanced accuracy score of 99.49% means that the machine can determine true postives (while factoring false negatives) and true negatives (while factoring false positives) around 99.5% of the time.
  - Precision
  The precision score for Machine 1 is 100% for predicting healthy loans (0) and 86% for predicting risky loans (1). The precision score determines whether or not a machine can predict True Positives while factoring the False Positives. While a 100% chance in predicting precision in healthy loans is excellent, an 86% chance for predicting precision in risky loans is only considered good -- and this would be the focus of the machine for the company.
  - Recall
  The recall score for Machine 1 is 99% for predicrting healthy loans (0) and 100% for predicting risky leans (1). The recall score determines whether or not a machine can predict True Positives while factoring the False Negatives. While a 99% chance in predicting precision in healthy loans is excellent, a 100% chance for predicting precision in risky loans is excellent. This score is important to the company but is not the main focus of the company in assessing risky loans.


## Summary

While both machines are overall very good for the company to determine the credit worthiness of borrowers (or predict risky loans). Machine 2 is performs better overall with a better recall score and balanced accuracy score. 


The most important part of the machine is to determine true positives and, fish out the false positives of risky loans. The peer to peer lending services seek to reduce as much risk as possible by flagging those loans that seem more risky than the others. This inherently means that the most important aspect of these machines are the precision scores.

Since both machines have good precision scores, I would recommend using the model. However, using model 2 is overall a better decision as the balanced accuracy score, and the recall score performs higher than model 1.
