# Loan Status Prediction using Logistic Regression

## Overview
This project involves building a logistic regression model to predict loan status, distinguishing between healthy loans (0) and high-risk loans (1). The dataset includes various features related to loan size, interest rates, borrower income, and more. The goal is to assess the model's performance in accurately classifying loan status.

## Dataset
The dataset used for this project contains 77,536 observations and the following features:

- `loan_size`: The size of the loan.
- `interest_rate`: The interest rate applied to the loan.
- `borrower_income`: The income of the borrower.
- `debt_to_income`: The ratio of the borrower’s debt to income.
- `num_of_accounts`: The number of accounts the borrower has.
- `derogatory_marks`: The number of derogatory marks on the borrower’s credit report.
- `total_debt`: The total debt of the borrower.
- `loan_status`: The target variable indicating whether the loan is healthy (0) or high-risk (1).

## Steps

### 1. Data Preparation
- **Separating Labels and Features**:
  - The target variable (`loan_status`) is separated as `y`.
  - The remaining features are assigned to `X`.

### 2. Data Splitting
- **Train-Test Split**:
  - The data is split into training and testing sets using an 80-20 split.
  - `train_test_split` is used with a `random_state` of 1 to ensure reproducibility.

### 3. Model Training
- **Logistic Regression Model**:
  - A logistic regression model is instantiated with the `lbfgs` solver and a `random_state` of 1.
  - The model is trained using the training data (`X_train`, `y_train`).

### 4. Model Evaluation
- **Model Scoring**:
  - The model’s performance is evaluated by scoring it on both the training and testing data.
  - Training Data Score: **0.9921**
  - Testing Data Score: **0.9918**

- **Predictions**:
  - Predictions are made on the test data (`X_test`).
  - The predictions are compared to the actual labels (`y_test`).

### 5. Performance Metrics
- **Confusion Matrix**:
  - A confusion matrix is generated to visualize the model's performance.
  - The confusion matrix is also presented as a heatmap for easier interpretation.

- **Classification Report**:
  - A detailed classification report is provided, showing the precision, recall, and F1-score for both classes (0 and 1).
  - The overall accuracy is **99%**, with a high precision and recall for both healthy and high-risk loans.

### 6. Conclusion
- **Model Performance**:
  - The logistic regression model performs well, with high accuracy in predicting both healthy and high-risk loans.
  - The precision and recall for high-risk loans (label 1) are slightly lower than for healthy loans (label 0), but still indicate strong performance.

### 7. Question
- **How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?**

**Answer**: The logistic regression model predicts healthy loans (label 0) with very high precision, recall, and F1-score. For high-risk loans (label 1), the model still performs well, with an F1-score of 0.88, indicating that while it may occasionally miss some high-risk loans (slightly lower recall), it generally does a good job of identifying them. The overall model accuracy is 99%, demonstrating robust performance in classifying loan status.

---

## How to Run the Code
1. Ensure you have the necessary Python packages installed:
   ```bash
   pip install pandas scikit-learn seaborn matplotlib
2. Load your dataset into a DataFrame called lending_data.
3. Follow the steps outlined in the code to train and evaluate the logistic regression model.

## Dependencies
Python 3.x
Pandas
Scikit-learn
Seaborn
Matplotlib

## Acknowledgements
This project is based on data analysis and model training techniques using Python and Scikit-learn. Special thanks to the developers and the community behind these powerful tools.
