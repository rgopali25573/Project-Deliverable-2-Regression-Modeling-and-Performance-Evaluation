# Project-Deliverable-2: Regression Modeling and Performance Evaluation

## Course
**MSCS-634-B01 – Advanced Big Data and Data Mining**

## Project Summary

This project focuses on developing and evaluating regression models to estimate healthcare billing costs using structured patient data. It is submitted as part of Deliverable 2 and demonstrates a complete regression workflow—from raw data preprocessing to model performance evaluation.

## Dataset Overview

The dataset includes features such as:

- Age
- Gender
- Medical Condition
- Insurance Provider
- Admission Type
- Billing Amount

Key preprocessing steps included text standardization, outlier filtering, and duplicate removal. Categorical data was one-hot encoded, and numerical data was standardized.

## Modeling Techniques

Three regression models were implemented:

- **Linear Regression**
- **Ridge Regression** (L2 regularization)
- **Lasso Regression** (L1 regularization)

These models were fitted on the training set after applying preprocessing and then evaluated using a separate test set.


## Evaluation Metrics

The models were assessed using:

- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R-Squared (R²)**
- **5-Fold Cross-Validated R²**


## Observations

- Minimal variation across the three models suggests limited predictive signal in the features.
- R² scores near zero and negative CV R² indicate the models were unable to explain the variance in billing amount effectively.
- Feature enrichment or more granular data may be necessary for improved prediction.


## Model Results

```
                      MSE       RMSE  R-Squared  CV R-Squared
LinearRegression  1.95e+08   13972.28       0.00         -0.00
RidgeRegression   1.95e+08   13972.28       0.00         -0.00
LassoRegression   1.95e+08   13972.28       0.00         -0.00
```


## Conclusion

Despite suboptimal performance, this project effectively demonstrates the process of building, validating, and comparing regression models in a healthcare cost prediction scenario. Future improvements should explore more informative features or alternate model families.
