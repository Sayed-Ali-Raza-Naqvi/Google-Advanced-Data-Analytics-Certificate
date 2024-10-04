# Predicting Generous Tippers: A Taxi Trip Data Analysis
## Overview
This project focuses on building machine learning models to predict generous tippers (customers tipping 20% or more) in NYC taxi trips. By analyzing data from the 2017 Yellow Taxi Trip Dataset, the goal is to assist cab drivers in identifying customers who are likely to tip generously. We use various models, including Random Forest and XGBoost, to predict the target variable: generous tippers.

## Objectives
- Data Exploration and Feature Engineering: Analyze the dataset and engineer meaningful features that contribute to predicting customer generosity in tipping.
- Model Training: Train models on the features extracted from the dataset.
- Model Evaluation: Assess the performance of models based on various metrics, including precision, recall, F1-score, and accuracy.
- Interpretation: Use model insights to identify key predictors of generous tippers.

## Feature Engineering
Several features were engineered to enhance model performance:

- Rush hour flags: am_rush, pm_rush columns indicating if the trip occurred during typical rush hours.
- Day and night flags: Categorizing rides into daytime and nighttime.
- Categorical features: Pickup and dropoff locations, rate code, and vendor were converted to dummy variables to facilitate model input.

## Modeling
Two machine learning models were employed in the analysis:

- ### Random Forest Classifier:
  - Hyperparameter tuning was performed using GridSearchCV with metrics like F1-score, accuracy, precision, and recall.
  - The model's ability to capture non-linear relationships in the data made it a good fit for this task.
- ### XGBoost Classifier:
  - Known for its gradient-boosted decision trees, this model was also optimized using GridSearchCV.
  - It is particularly effective for large datasets with complex relationships between features.

## Performance Metrics:
To evaluate the models, the following metrics were used:

- Accuracy: Measures the overall correctness of the model's predictions.
- Precision: Focuses on minimizing false positives (predicting a generous tip when there isn't one).
- Recall: Captures the model's ability to find all true generous tippers.
- F1-score: Balances precision and recall, considering both false positives and false negatives.
Given the even stakes between taxi drivers and customers, F1-score was selected as the primary metric for tuning the models.
