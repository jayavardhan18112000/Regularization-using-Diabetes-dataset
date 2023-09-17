# Diabetes Regression with Regularization Techniques

This project focuses on using regularization techniques like Lasso, Ridge, and Elastic Net to predict diabetes progression based on various features. The dataset used for this analysis is the Diabetes dataset from the Scikit-Learn library.

## Table of Contents
- [Introduction](#introduction)
- [Dataset Overview](#dataset-overview)
- [Data Preprocessing](#data-preprocessing)
- [Regularization Techniques](#regularization-techniques)
- [Model Evaluation](#model-evaluation)
- [Analysis of Non-Zero Coefficients](#analysis-of-non-zero-coefficients)
- [Conclusion](#conclusion)

## Introduction

In this project, we explore the application of regularization techniques to improve the performance of a regression model predicting diabetes progression. We specifically use Lasso, Ridge, and Elastic Net regularization methods to achieve this.

## Dataset Overview

The Diabetes dataset from Scikit-Learn is used for this project. It contains ten baseline variables, age, sex, BMI, average blood pressure, and six blood serum measurements for 442 diabetes patients. The target variable is a quantitative measure of disease progression one year after baseline.

## Data Preprocessing

- The dataset is loaded using Scikit-Learn's `load_diabetes` function.
- Features are standardized to have a mean of 0 and a standard deviation of 1 using `StandardScaler`.
- Polynomial features of degree 2 are generated using `PolynomialFeatures`.

## Regularization Techniques

### Lasso Regression
- LassoCV is employed to perform Lasso regression with cross-validated alpha values.
- The optimal alpha value is determined to be 4.417.
- The model is trained and evaluated.

### Ridge Regression
- RidgeCV is used to perform Ridge regression with cross-validated alpha values.
- The optimal alpha value is determined to be 40.0.
- The model is trained and evaluated.

### Elastic Net Regression
- ElasticNetCV is applied to perform Elastic Net regression with cross-validated alpha values.
- The model is trained and evaluated.

## Model Evaluation

- Model performance is evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²) values.

## Analysis of Non-Zero Coefficients

- After applying Lasso, Ridge, and Elastic Net regularization, the number of non-zero coefficients is recorded for each technique.
- for Ridge, there are 65 non zero coefficients
- for Lasso, there are 11 non zero coefficients
- for Elastic, there are 16 non zero coefficients

## Conclusion

This project demonstrates the application of Lasso, Ridge, and Elastic Net regularization techniques to predict diabetes progression. Elastic Net showed the highest R² value, indicating the best fit for the data. Analysis of non-zero coefficients revealed interesting insights into feature importance and model complexity.

Feel free to clone this repository and explore the code to gain a deeper understanding of the process and results.
