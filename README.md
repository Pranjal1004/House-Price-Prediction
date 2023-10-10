# House-Price-Prediction
## Regression Project:
To predict the prices of houses based on certain features.

## Models Used:
Multiple Linear Regression, XGBoost & Random Forest Regressor (Best)

## Files Description:

• train.csv - the training set (1460 rows x 81 columns)

• test.csv - the test set (1459 rows x 80 columns), has no target variable

• final_submission_test_dataset.csv - Contains the predicted values of "test.csv" dataset which were predicted using the model trained

   on "train.csv" dataset (1459 rows x 2 columns: one col is "House Id" and other is "Sale Price" for each house)

## Main Highlights:
• Used Standard Scaler for Feature Scaling, One Hot Encoding to convert categorical variables to Numerical Variables

• Dealt with null values: 

  ⦾ Removed All those columns which have more than 50 % null values 
    
  ⦾ Used "mean" to fill null values in remaining numerical variables 
  
  ⦾ Used "mode" to fill null values in remaining categorical variables variables 

• Considered r2_score to pick the best model, which was Random Forest Regressor with an r2_score of 0.8284 or 82.84 %

• Did "Hyper Parameter Tuning" using "Randomized Search" to find the best parameters for Random Forest Regressor, which gave the r2 Score of 0.8439 or 84.39 %

• Best hyper parameters were {'n_estimators': 1200, 'min_samples_split': 2, 'min_samples_leaf': 1, 'max_features': 'sqrt', 'max_depth': 50, 'bootstrap': False}

## Source of Dataset:
https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data?select=train.csv


