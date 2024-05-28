# Decision Tree and Bootstrap Aggregated Forest on Synthetic Data

This notebook demonstrates the application of Decision Tree Regressor and a Bootstrap Aggregated Forest (Bagging Regressor) on a synthetic dataset. The dataset consists of both important and random features generated using various distributions. The goal is to highlight the importance of hyperparameter tuning and evaluate its performance.

## Table of Contents
- [Introduction](#introduction)
- [Data Generation](#data-generation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)
- [Dependencies](#dependencies)

## Introduction
This notebook demonstrates the use of Decision Tree Regressor on a synthetic dataset. The dataset is designed to contain both significant and random features generated using different statistical distributions. The objective is to visualize the correlation matrix of the features, train a Decision Tree Regressor to predict the target variable `Y`, and evaluate the model's performance. And then perform the hyperparameter tuning to find out the optimal values. Atlast comparing the single decision tree with ensemble trees using Bagging Regressor.

## Data Generation
We generate a synthetic dataset with the following features:
- `important_feature_poisson`: Poisson-distributed feature.
- `important_feature_dummy`: Binomial-distributed dummy feature.
- `random_feature_normal`: Normally distributed feature.
- `random_feature_dummy`: Binomial-distributed dummy feature.

The target variable `Y` is generated as a combination of `important_feature_poisson` and `important_feature_dummy`.

## Exploratory Data Analysis (EDA)
We perform EDA to understand the dataset better:
- Visualize the correlation matrix of the features.
- Generate scatter plots to observe relationships between features and the target variable.

## Model Training
We train a Decision Tree Regressor on the synthetic dataset:
- Split the data into training and testing sets.
- Train a Decision Tree Regressor with default parameter and evaluate.
- Perform hyperparameter tuning for the decision tree and evaluate the model to find out the optimal parameter values.
- Additionally, train a Bagging Regressor (Bootstrap Aggregated Forest) to improve the model's robustness.

## Model Evaluation
The models are evaluated using the following metrics:
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)

We compare the performance of the Decision Tree Regressor and the Bagging Regressor.

## Conclusion
The notebook concludes with a summary of the model performances, highlighting the effectiveness of using a Bagging Regressor for reducing variance and improving prediction accuracy on synthetic data.

## Dependencies
The notebook requires the following libraries:
- `math`
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
