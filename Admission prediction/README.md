#  Admission Prediction using Machine Learning

##  Project Overview

This project focuses on predicting the **chance of admission** for students based on various academic and profile features such as GRE score, TOEFL score, CGPA, SOP, and more.

The goal was to **compare multiple machine learning models** and identify which performs best on tabular data.

---

##  Dataset

* **Name:** Graduate Admission Dataset
* **Type:** Regression
* **Target Variable:** Chance of Admit

### Features:

* GRE Score
* TOEFL Score
* University Rating
* SOP
* LOR
* CGPA
* Research

---

##  Models Used

The following models were trained and compared:

* Linear Regression
* Ridge Regression
* Lasso Regression
* Decision Tree Regressor
* Random Forest Regressor
* Support Vector Regressor (SVR)
* XGBoost Regressor

---

##  Approach

1. Data preprocessing
2. Train-test split
3. Model training using a loop
4. Evaluation using:

   * R² Score
   * Mean Squared Error (MSE)
5. Comparison of results

---

##  Results

| Model             | R² Score | MSE    |
| ----------------- | -------- | ------ |
| Linear Regression | 0.818    | 0.0037 |
| Ridge             | 0.818    | 0.0037 |
| Random Forest     | 0.791    | 0.0042 |
| SVR               | 0.758    | 0.0049 |
| XGBoost           | 0.746    | 0.0051 |
| Decision Tree     | 0.578    | 0.0086 |
| Lasso             | -0.007   | 0.0205 |

---

##  Key Insights

*  **Linear Regression performed the best**, indicating the data has a strong linear relationship
*  Complex models like XGBoost did not outperform due to:

  * Small dataset size
  * Lack of hyperparameter tuning
*  Lasso performed poorly due to aggressive feature shrinking
*  Decision Trees overfitted the data

---

##  Conclusion

For this dataset:

* Simple models
