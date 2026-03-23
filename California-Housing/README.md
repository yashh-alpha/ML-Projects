# California Housing Price Prediction

## Project Overview

This project focuses on predicting housing prices using the California Housing dataset. The goal is to analyze the data, understand feature relationships, and compare the performance of multiple machine learning models on a regression task.

---

## Dataset

* Source: Scikit-learn (`fetch_california_housing`)
* Type: Regression
* Target Variable: Median house value

### Features:

* MedInc: Median income
* HouseAge: Median house age
* AveRooms: Average number of rooms
* AveBedrms: Average number of bedrooms
* Population
* AveOccup: Average occupancy
* Latitude
* Longitude

---

## Exploratory Data Analysis

The dataset was analyzed to understand:

* Distribution of features
* Correlation between variables
* Relationship between features and target

### Key Observations:

* Median income has the strongest correlation with house prices
* Several features show non-linear relationships with the target
* No missing values were present in the dataset

---

## Models Used

The following regression models were implemented and compared:

* Linear Regression
* Ridge Regression
* Lasso Regression
* Decision Tree Regressor
* Random Forest Regressor
* Support Vector Regressor (SVR)
* XGBoost Regressor

---

## Evaluation Metrics

* R² Score
* Mean Squared Error (MSE)

---

## Results

| Model             | R² Score | MSE  |
| ----------------- | -------- | ---- |
| XGBoost           | 0.83     | 0.22 |
| Random Forest     | 0.80     | 0.25 |
| SVR               | 0.72     | 0.35 |
| Decision Tree     | 0.61     | 0.50 |
| Ridge             | 0.57     | 0.55 |
| Linear Regression | 0.57     | 0.55 |
| Lasso             | ~0.00    | 1.31 |

---

## Key Insights

* Tree-based models significantly outperformed linear models
* XGBoost achieved the best performance due to its ability to capture non-linear relationships and feature interactions
* Linear models underperformed, indicating that the dataset is not purely linear
* Decision Trees showed signs of overfitting compared to ensemble methods

---

## Conclusion

This project demonstrates that model performance depends on the nature of the data. For datasets with complex and non-linear relationships, ensemble methods such as XGBoost and Random Forest are more effective than linear models.

---

## Tools and Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Matplotlib
* Seaborn

---

## Author

Yash
