
# Project 2: Ames, Iowa Housing Price Prediction
by Nati Marcus

## Problem Statement
Given the Ames housing dataset, how well can I predict house prices for Ames on unseen data? To answer this question I will be conducting Linear Regression Analysis to calculate the root mean squared error (RMSE) for housing prices. Doing so will allow me to evaluate around how accurate in dollars the prediction is. I will be comparing this figure to the "baseline model" RMSE, i.e the average error if you were to predict the median housing price of the training data.

## Data Overview
All of the analysis will be conducted on training data from the `'train.csv'` file. This dataset contains 2051 observations and has 81 features, including the `SalesPrice` outcome variable. Around half of the features are numerical and the other half are categorical. After Regression is conducted on the training dataset, the model will be used on the test data (`'test.csv'`) to predict house price.

## Data Dictionary
A detailed data dictionary is available on kaggle at this [link](https://www.kaggle.com/c/dsi-ames/data)

## Analysis Overview
Using a generalized regression function I created, and various feature engineering methods, I trained 6 Linear Regression models. The results from the 5th model yielded the best result in terms of RMSE. This model contained polynomial features for numerical values that showed potential to be good estimators using pairplots and a heatmap. It also contained various dummy variables for metrics such as the overall quality rating of the house or the type of heating in the house. On the training data, the RMSE for this model using scaled data was \\$31,752.33. On the test data, the RMSE for this model was \\$ 27,977.02.

## Conclusions and Recommendations
The model I constructed yielded a signifcantly better RMSE result compared to the baseline model RMSE on both the training and testing data. However, the model is still not as accurate as it could be, so I would suggest using a more systematic approach to selecting features in order to optimize this model. In conclusion, the model is a good start, but more work needs to be done to obtain a more accurate house price prediction.
