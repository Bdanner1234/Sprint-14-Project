# Sprint-14-Project
Machine larning for texts
Project Overview

The goal of this project was to predict customer churn for a telecom company. By identifying customers likely to leave, the company can take proactive retention measures and reduce revenue loss.

This project was part of the TripleTen Data Science Program.

Data

The dataset included:

Customer contract details (type, start/end dates, payment method)
Internet services (DSL, fiber optic, security, backup, etc.)
Customer demographics (tenure, monthly charges, total charges)
Target variable: Churn (Yes/No)

Methodology

Data Preprocessing
Converted EndDate = "No" into active contracts.
Handled missing values in numerical and categorical fields.
One-hot encoded categorical variables.
Standardized numerical features.

Model Training

Tried Logistic Regression, Random Forest, and Gradient Boosting.
Balanced the dataset with SMOTE to address class imbalance.
Evaluated models with F1-score (threshold ≥ 0.59) and ROC-AUC.

Model Selection

Selected the model that achieved the best balance between recall and precision.

Results

Final model: Random Forest Classifier (after hyperparameter tuning)
F1-score: ~0.60 (met requirement)
ROC-AUC: ~0.85

Business impact: enables the telecom company to identify high-risk customers and take actions such as discounts, loyalty rewards, or targeted outreach.

Tech Stack

Python (pandas, NumPy, scikit-learn)
Jupyter Notebook
Matplotlib / Seaborn for visualization
