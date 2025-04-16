# Insurance Charges Prediction

## Project Overview

This project focuses on predicting the **insurance charges** of individuals based on various features such as **age**, **bmi**, **smoker status**, **region**, and others. The goal is to apply machine learning techniques, including **data preprocessing**, **feature engineering**, and **model evaluation**, to build a predictive model. We explore both **Linear Regression** and **Polynomial Regression** models to compare performance and understand the impact of different approaches on prediction accuracy.

---

### Set up the virtual environment in the terminal:
``` shell
python3 -m venv .venv
```
Activate the virtual enivronment
``` shell
source .venv/bin/activate
```

Install requirements
``` shell
py -m pip install -r requirements.txt
```

Link to notebook: https://github.com/Crusoe22/ml_regression_moss/blob/main/regression_moss.ipynb  
Link to peer review: https://github.com/Crusoe22/ml_regression_moss/blob/main/peer_review.md 




## Dataset

The dataset used in this project is the **insurance.csv** dataset, which contains the following features:

- **age**: The age of the individual.
- **sex**: The gender of the individual (male/female).
- **bmi**: The body mass index (BMI) of the individual.
- **children**: The number of children/dependents covered by the individual’s insurance.
- **smoker**: Whether the individual is a smoker (yes/no).
- **region**: The region of the individual (northeast, southeast, southwest, northwest).
- **charges**: The insurance charges incurred by the individual (target variable).

---

## Results

### Pipeline 1: Linear Regression
- **R²**: 0.796
- **RMSE**: 5583.31
- **MAE**: 4136.42

### Pipeline 2: Polynomial Regression (degree=3)
- **R²**: 0.903
- **RMSE**: 3847.75
- **MAE**: 2563.74

The **Polynomial Regression** model (degree=3) outperformed the **Linear Regression** model in all evaluation metrics, indicating that capturing non-linear relationships between the features and target variable led to better predictions.

---