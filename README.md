# Spam Email Detection using Machine Learning

## Background

As part of an initiative at an Internet Service Provider (ISP) to improve customer satisfaction and security, a project has been developed to enhance the email filtering system by accurately detecting and filtering spam emails using supervised machine learning techniques.

## Objective

The objective of this project is to develop and compare two different machine learning models, logistic regression and random forest, to determine which is more effective at identifying spam emails. These models will be trained and evaluated using a dataset labeled as spam or not spam.

## Instructions

### Split the Data into Training and Testing Sets

1. **Read the Data**:
   - Download and read the dataset from `https://static.bc-edx.com/mbc/ai/m4/datasets/spam-data.csv` into a Pandas DataFrame.

2. **Prediction**:
   - In the provided markdown cell in the starter notebook, make a prediction as to which model (logistic regression or random forest) you expect will perform better.

3. **Prepare the Data**:
   - Extract the 'spam' column as the labels set (y).
   - Create a features DataFrame (X) from the remaining columns.
   - Note: A '0' in the “spam” column indicates a legitimate message, and a '1' indicates spam.
   - Use the `value_counts` function to check the balance of the labels.

4. **Split the Data**:
   - Use `train_test_split` to divide the data into training and testing datasets.

### Scale the Features

1. **Standard Scaling**:
   - Create an instance of `StandardScaler`.
   - Fit the scaler using the training data.
   - Transform both the training and testing feature sets using the fitted scaler.

### Create a Logistic Regression Model

1. **Model Fitting**:
   - Fit a logistic regression model using the scaled training data (X_train_scaled and y_train) with `random_state` set to 1.

2. **Testing and Evaluation**:
   - Predict the testing data labels using the scaled testing feature data (X_test_scaled).
   - Calculate and report the accuracy score of the model.

### Create a Random Forest Model

1. **Model Fitting**:
   - Fit a random forest classifier using the scaled training data.

2. **Testing and Evaluation**:
   - Predict the testing data labels using the scaled testing feature data.
   - Calculate and report the accuracy score of the model.

### Evaluate the Models

1. **Comparison**:
   - In the designated markdown cell, analyze which model performed better and discuss how this compares to your initial prediction.

### Reference

Hopkins, M., Reeber, E., Forman, G. & Suermondt, J. 1999. Spambase [Dataset]. UCI Machine Learning Repository. Available: https://archive.ics.uci.edu/dataset/94/spambase