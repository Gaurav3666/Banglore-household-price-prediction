# Banglore-household-price-prediction
# 🏠 House Price Prediction using Machine Learning

## 📌 Project Overview
This project aims to predict house prices using Machine Learning techniques.  
The model is trained on cleaned real estate data by applying proper preprocessing, outlier removal, and feature engineering.

The goal of this project is to understand the **end-to-end ML workflow**, including:
- Data cleaning
- Feature scaling
- Encoding categorical variables
- Model training
- Model evaluation

---

## 🧠 Problem Statement
House prices depend on multiple factors such as:
- Location
- Total square feet area
- Number of bedrooms (BHK)
- Number of bathrooms
- Balcony count

The objective is to build a regression model that can accurately predict house prices based on these features.

---

## 🗂 Dataset Description
The dataset contains the following features:

| Column Name | Description |
|------------|-------------|
| location | Area where the house is located |
| total_sqft | Total area of the house |
| bhk | Number of bedrooms |
| bath | Number of bathrooms |
| balcony | Number of balconies |
| price | House price (target variable) |
| Price_per_sqft | Derived feature (price / total_sqft) |

---

## 🧹 Data Cleaning & Preprocessing
The following preprocessing steps were performed:

- Removed outliers using Z-Score / Standard Deviation Method 
- Grouped rare locations into a single category (`other`)
- Removed illogical outliers using **BHK-based price comparison**
- Applied **StandardScaler** to numerical features
- Applied **OneHotEncoder** to categorical features
- Used **Pipeline and ColumnTransformer** to avoid data leakage

---

## ⚙️ Technologies & Libraries Used
- Python
- NumPy
- Pandas
- Scikit-learn

Key sklearn modules:
- `train_test_split`
- `LinearRegression`
- `StandardScaler`
- `OneHotEncoder`
- `Pipeline`
- `ColumnTransformer`
- `r2_score`, `mean_absolute_error`

---

## 🤖 Model Used
- **Linear Regression**

The model was trained using a clean and scaled dataset to ensure better convergence and performance.

---

## 📊 Model Evaluation
The model was evaluated using:
- **R² Score** – to measure how well the model explains the variance
- **Mean Absolute Error (MAE)** – to understand average prediction error

---

## ✅ Results
- The dataset was successfully cleaned and standardized
- Outliers were significantly reduced
- The model achieved stable and realistic predictions
- Suitable for beginner to intermediate ML learning

---

## 🚀 Future Improvements
- Add Ridge and Lasso Regression
- Perform Cross-Validation
- Try advanced models like Random Forest or XGBoost
- Deploy the model using Flask or FastAPI

---

## 🙋‍♂️ Author
**Gaurav Kumar**  
Aspiring Data Scientist | Machine Learning Enthusiast

---

## 📌 Note
This project is created for learning purposes and to understand real-world data preprocessing and machine learning workflows.
