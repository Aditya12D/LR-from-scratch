# Linear Regression Models from Scratch

This repository contains Python implementations of **Simple Linear Regression** and **Multiple Linear Regression** from scratch, alongside comparisons with scikit-learn models and visualizations for conceptual clarity.

## 📂 Files

| File                          | Description                                                                                                                      |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| `simplelinearregression.py`   | Implements simple linear regression without libraries and validates with scikit-learn.                                           |
| `multiplelinearregression.py` | Implements multiple linear regression (Normal Equation), compares with scikit-learn, and visualizes regression hyperplane in 3D. |

## 🔧 Features

✅ Builds regression models **from scratch** (no direct ML libraries)
✅ Compares results with scikit-learn models
✅ Visualizes regression line and hyperplane
✅ Uses real-world datasets with numerical and categorical features

## 📊 Datasets

1. **Study\_vs\_Score\_data.csv** – For simple regression with:

| Attendance\_Hours | Final\_Marks |
| ----------------- | ------------ |

2. **multiple\_linear\_regression\_dataset.csv** – For multiple regression with:

| age | experience | income |
| --- | ---------- | ------ |

3. **Student\_Performance.csv** – For multiple regression with categorical encoding.

> ⚠️ **Note:** Adjust dataset paths in scripts as per your directory structure.

## 📈 Outputs

* **Simple Linear Regression:** Regression line over scatter plot predicting Final Marks from Attendance Hours.
* **Multiple Linear Regression:**

  * Predictions from custom and scikit-learn models
  * 3D regression hyperplane plots for age, experience, and income data
  * Encoded features analysis for student performance

## 📝 Key Learnings

* Deriving slope and intercept for simple linear regression
* Implementing **Normal Equation** for multiple linear regression:

  $$
  \beta = (X^TX)^{-1}X^Ty
  $$
* Using `np.linalg.inv()` for matrix inversion in the Normal Equation solution
* Understanding **matrix differentiation** to derive the Normal Equation, where setting the derivative of the cost function to zero yields the closed-form solution
* Handling categorical features using `OneHotEncoder`
* Visualizing high-dimensional regression models

## ✨ Future Improvements

* Implement **gradient descent optimization**
* Extend to **polynomial regression**
* Integrate evaluation metrics (RMSE, R² score) in outputs
