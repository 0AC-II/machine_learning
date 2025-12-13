# Diabetes Prediction Using Logistic Regression

This project applies logistic regression to predict the likelihood of diabetes using clinical and demographic features. The goal is to build an interpretable baseline model while demonstrating a complete machine learning workflow, from data exploration to evaluation and interpretation.

## Dataset
The dataset contains 768 patient records with the following features:
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thickness
- Insulin
- BMI
- Diabetes Pedigree Function
- Age

The target variable is **Outcome**, where:
- 0 = Non-diabetic
- 1 = Diabetic

## Exploratory Data Analysis
Initial analysis revealed:
- Several features contain zero values that are biologically implausible (e.g., glucose, insulin), highlighting data quality limitations.
- The dataset is moderately imbalanced, with more non-diabetic cases than diabetic cases.
- Glucose, BMI, and Age show stronger correlations with the target variable compared to other features.

Visualizations included feature distributions, a correlation heatmap, and class balance inspection.

## Model
A **Logistic Regression** model was trained due to its:
- Interpretability
- Suitability for binary classification
- Ability to provide meaningful feature coefficients

The data was split into training and test sets before model fitting.

## Evaluation
Model performance on the test set:
- Accuracy: ~75%
- ROC AUC: ~0.82

The confusion matrix and classification report show:
- Better performance on non-diabetic cases
- Moderate recall for diabetic cases, reflecting class imbalance

## Feature Importance
Model coefficients indicate:
- **Glucose** as the strongest predictor
- **BMI** and **Age** as significant contributing factors
- Genetic and reproductive factors playing secondary roles

These findings align well with established medical knowledge.

## Conclusion
Despite its simplicity, logistic regression provided strong baseline performance and clear interpretability. This project demonstrates how thoughtful data exploration and evaluation can produce reliable and explainable machine learning models in healthcare.

Future improvements may include feature engineering, handling zero-inflated values, class balancing techniques, and experimenting with more complex models.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
