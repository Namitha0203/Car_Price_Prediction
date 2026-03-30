# 🚗 Car Price Prediction — Machine Learning Project

A machine learning project to predict used car prices based on features such as brand, model, year, mileage, fuel type, transmission, and more.  
Multiple regression models were trained, evaluated, and compared. Hyperparameter tuning was performed to improve model performance.

---

## 📌 Project Overview

The goal of this project is to build a predictive model that estimates the selling price of a car using supervised machine learning techniques.  
The workflow includes data preprocessing, feature engineering, model training, evaluation, and hyperparameter tuning.

---


---

## 🧹 Data Preprocessing

Key preprocessing steps:

- Handling missing values  
- Encoding categorical variables  
- Feature scaling (for SVR)  
- Outlier handling  
- Train-test split  

---

## 🤖 Models Used

The following machine learning models were trained:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Gradient Boosting Regressor  
- Support Vector Regressor (SVR)

---

## 📊 Model Performance (Before Tuning)

| Model | MAE | RMSE | R² |
|-------|------|--------|-------|
| Gradient Boosting | 1050.68 | 1396.63 | 0.9632 |
| Random Forest | 1056.04 | 1491.11 | 0.9580 |
| Decision Tree | 1160.58 | 1722.07 | 0.9440 |
| Linear Regression | 1469.99 | 2058.77 | 0.9200 |
| SVR | 5114.24 | 7615.59 | -0.0951 |

Gradient Boosting performed the best among all baseline models.

---

## 🔧 Hyperparameter Tuning (Gradient Boosting)

GridSearchCV was used to tune:

- `n_estimators`
- `learning_rate`
- `max_depth`
- `subsample`

The tuned Gradient Boosting model achieved improved MAE, RMSE, and R² compared to the baseline.

---

## 🏆 Best Model

After tuning, **Gradient Boosting Regressor** remained the top-performing model with:

- Lower prediction error  
- Better generalization  
- Higher R² score  

---


