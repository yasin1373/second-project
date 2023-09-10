# Lasso Regression Pipeline

This project implements a machine learning pipeline for Lasso regression using sklearn. It evaluates model performance through k-fold cross-validation on a dataset with 16 input variables and 1 target variable.

## Overview

Lasso regression is a linear model that performs feature selection and regularization to prevent overfitting. This analysis builds a pipeline to standardize the data, reduce dimensionality with PCA, then train a Lasso model.

Cross-validation provides an estimate of out-of-sample performance for each model. The pipeline is executed repeatedly to evaluate different configurations of the Lasso regression.

## Code Overview

The main steps are:

- Import libraries (pandas, sklearn)
- Load and prepare input (X) and target (y) data 
- Define pipeline with scaling, PCA, and Lasso steps
- Create a dictionary of pipeline variants 
- Function to evaluate model with cross-validation
- Fit and evaluate each pipeline
- Print cross-validation MSE 

## Results

The output shows cross-validated mean squared error for each Lasso regression model. Lower values indicate better performance. The results can be used to select the optimal model configuration.

## Usage

To reproduce the analysis, run the Jupyter notebook. The input data file must be formatted with 16 feature columns and 1 target column.

This code provides a template for evaluating sklearn pipelines with cross-validation. It can be adapted for other regression models and datasets.

