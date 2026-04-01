# Student Burnout Prediction - A Critical Look at Synthetic Data

Exploratory data analysis and ML classification pipeline built in R and Python, 
connected via the `reticulate` package and delivered as an interactive Quarto report.

# Project Overview

This project investigates whether student burnout level can be predicted from 
academic and lifestyle factors such as study hours, sleep, stress, and attendance. 
The analysis reveals that the dataset's synthetic nature makes prediction impossible 
at above-chance levels - a finding that is itself the main contribution of this work.

# Models Used

| Model               | Accuracy |
|---------------------|----------|
| Logistic Regression | ~33.3%   |
| Random Forest       | ~33.3%   |
| XGBoost             | ~33.3%   |

All three models performed at random baseline, confirming near-zero correlation 
between features and the target variable.

# Tech Stack

- R - data exploration, visualizations (ggplot2, corrplot)
- Python - machine learning (scikit-learn, XGBoost)
- reticulate - R/Python integration
- **Quarto - report generation 

# Key Finding

A high usability score on Kaggle does not guarantee predictive utility. 
Burnout labels in this dataset were assigned independently of feature values, 
making ML prediction fundamentally impossible on this data.
