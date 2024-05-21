# Classification Models for Credit Card Default Prediction

This repository contains the implementation and optimization of several classification models to predict credit card default using the "default of credit card clients" dataset.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Setup](#setup)
- [Pre-processing](#pre-processing)
- [Model Implementation](#model-implementation)
- [Hyperparameter Optimization](#hyperparameter-optimization)
- [Evaluation](#evaluation)
- [Univariate Analysis](#univariate-analysis)
- [Results](#results)
- [Contributing](#contributing)

## Overview

The goal of this project is to build and optimize classification models to predict whether a client will default on their credit card payment next month. The models implemented include Logistic Regression, Random Forest, Support Vector Classifier (SVC), XGBoost, LightGBM, and a Stacking Classifier.

## Dataset

The dataset used is "default of credit card clients.xls" which contains 30,000 observations and 25 features. The target variable is whether the client will default on their credit card payment next month.

## Setup

1. Clone the repository:
    ```sh
    git clone https://github.com/Ismat-Samadov/Classification_Modells.git
    cd Classification_Modells
    ```

2. Install the required libraries:
    ```sh
    pip install -r requirements.txt
    ```

3. Place the dataset `default of credit card clients.xls` in the root directory of the repository.

## Pre-processing

The pre-processing steps include:
- Handling missing values.
- Encoding categorical variables.
- Scaling numerical features.
- Splitting the data into training and testing sets.

## Model Implementation

The following models are implemented:
- **Logistic Regression**
- **Random Forest**
- **Support Vector Classifier (SVC)**
- **XGBoost**
- **LightGBM**
- **Stacking Classifier**

Each model is evaluated using accuracy and F1 score.

## Hyperparameter Optimization

Optuna is used for hyperparameter optimization. The objective functions for each model are defined, and the best parameters are obtained through multiple trials.

## Evaluation

The performance of all models is compiled into a DataFrame for easy comparison. The results include both the accuracy and F1 score for each model.

## Univariate Analysis

Univariate analysis is performed on the best model (LightGBM in this case) to understand the importance of each feature.

## Results

The final results after optimization for the LightGBM model are:
- **Optimized LightGBM Accuracy:** 0.816
- **Optimized LightGBM F1 Score:** 0.4682

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements.