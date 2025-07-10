# 🏡 House Price Prediction using Machine Learning

This project demonstrates how machine learning models can be used to predict house prices based on various features. Three regression models are used and evaluated:
- **Linear Regression**
- **Random Forest Regressor**
- **XGBoost Regressor**

Two preprocessing approaches are applied:
1. **Standard preprocessing** (imputation, scaling, encoding)
2. **Preprocessing with Outlier Removal** using IQR (Interquartile Range)

---

## 📊 Dashboard Overview

The project includes performance comparison of models in terms of:
- **R² Score**
- **RMSE (Root Mean Squared Error)**
- **MSE (Mean Squared Error)**

---

## 🧠 Models Used

| Model              | Description                                              |
|-------------------|----------------------------------------------------------|
| Linear Regression  | A baseline model to understand linear relationships     |
| Random Forest      | Ensemble method using decision trees with bagging       |
| XGBoost            | Gradient boosting model with regularization capabilities|

---

## 📁 Project Structure

House-Price-Prediction/
├── house_price_prediction_standard.ipynb # Standard preprocessing
├── house_price_prediction_no_outliers.ipynb # Preprocessing with outlier removal
├── df_train.csv # Dataset (sample or real)
├── model_comparison.png # R² bar chart visualization
└── README.md # Project documentation


---

## 📂 Dataset

The dataset (`df_train.csv`) contains house-related features such as:
- `living_in_m2`
- `bathrooms`
- `bedrooms`
- `location`
- `price` (target variable)

Preprocessing includes:
- Log transformation on `price` and `living_in_m2`
- Missing value handling using `SimpleImputer`
- Scaling numeric features
- Encoding categorical features with `OneHotEncoder`
- Outlier removal using IQR (optional)

---

## 📉 Model Performance (With Outlier Removal)

![image](https://github.com/user-attachments/assets/c29a6f54-25bf-4640-9f0f-ff929fcc10c0)



| Model              | R² Score | RMSE | MSE  |
|-------------------|----------|------|------|
| Linear Regression | 0.76     | 0.40 | 0.16 |
| Random Forest     | 0.80     | 0.35 | 0.12 |
| XGBoost           | 0.79     | 0.36 | 0.13 |

> _Note: Results are based on preprocessed data and may vary based on feature selection and hyperparameters._

---

## ⚙️ How to Use

### 1. Clone the repository

```bash
git clone [https://github.com/yourusername/House-Price-Prediction.git](https://github.com/MuhammadOmama/House-Price-Prediction-using-Machine-Learning
cd House-Price-Prediction
```


### 2. Installation Command for Users
pip install -r requirements.txt


