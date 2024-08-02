# Module 12 Report Template

## Overview of the Analysis

This report presents the methodologies employed to train and assess a model designed to evaluate loan risk. Utilizing a historical dataset from a peer-to-peer lending services company, the model aims to accurately determine the creditworthiness of borrowers.

* The dataset included two measurable variables: 0 (healthy loan) and 1 (high-risk loan). In total, there were 75,036 instances labeled as healthy loans and 2,500 instances labeled as high-risk loans.

* The stages of machine learning process involved through this analysis:
    * Spliting the data into training and testing sets. 
    * Creating a Logistic Regression Model with the original data.
    
## Results

* Variable 0 (Healthy Loan):

    * The model is extremely accurate in predicting healthy loans, as indicated by a precision of 1.00 and a recall of 0.99. This means almost all healthy loans are correctly identified, with very few false positives.

* Variable 1 (High-risk Loan)
    * The model shows good performance in predicting high-risk loans with a precision of 0.85 and recall of 0.91. This indicates that while most high-risk loans are correctly identified, there are still some that are missed (false negatives), and some healthy loans are incorrectly predicted as high-risk (false positives).

## Summary

The logistic regression model performs excellently in predicting healthy loans and reasonably well for high-risk loans. While the high-risk loan predictions are not as precise as the healthy loans, they are still quite reliable with good precision and recall values. The model's overall accuracy and the balanced F1-scores further indicate a strong performance. Based on this analysis, the model for healthy loans is recommended.
