# Ames Housing Price Prediction

A machine learning project exploring what drives home prices and how well different models can predict them.

## Overview

This project uses the Ames Housing dataset to model residential property prices using a full data-science workflow: cleaning, exploratory analysis, feature engineering, baseline modeling, and ensemble learning. The goal is to identify the features that matter most in price determination and to compare how different algorithms perform on a structured, real-world dataset.

## Objectives

- Understand the structure and quirks of the Ames dataset

- Explore relationships between key housing features and sale price

- Build and evaluate predictive models (Linear Regression, Decision Tree, Random Forest)

- Interpret feature importance and connect it with real housing-market intuition

- Present findings in a clear, reproducible format

## Dataset

The Ames Housing dataset contains 1400+ residential property records from Ames, Iowa, with detailed information on structural attributes, quality, size, and lot characteristics.
Variables include:

- OverallQual (overall material and finish quality)

- GrLivArea (above-ground living area)

- 2ndFlrSF (second-floor square footage)

- Garage, basement, exterior, and neighborhood descriptors

- Sale conditions and final SalePrice

## Methodology

The workflow includes:

- Data cleaning — handling missing values, converting categorical features, and removing outliers.

- Exploratory analysis — distribution checks, correlation heatmaps, and scatter relationships.

- Baseline modeling — Linear Regression to establish a performance reference.

- Tree-based modeling — Decision Tree and Random Forest for nonlinear relationships.

- Evaluation — MSE, RMSE, and R² score on a held-out test set.

- Interpretation — Feature importance and prediction-vs-actual diagnostics.

## Results

- Linear Regression: R² ≈ 0.35

- Decision Tree: R² ≈ 0.77

- Random Forest: R² ≈ 0.876, RMSE ≈ 28,162

The Random Forest model performed best, capturing both dominant patterns and subtler interactions within the data. The top predictors — OverallQual, GrLivArea, and 2ndFlrSF — align with market intuition about the impact of build quality and living space on home value.

## Key Insights

- Housing prices in Ames are heavily influenced by material quality and usable square footage.

- Nonlinear models offer significant improvements over simple linear approaches for this dataset.

- Ensemble methods provide stability and interpretability through feature importance rankings.

- Prediction-vs-actual plots show tight clustering around the ideal line, indicating reliable generalization.
