# 🏠 House Price Prediction in King County

This project focuses on predicting house prices in King County (Seattle and surrounding areas) using machine learning. We analyzed data from **May 2014 to May 2015** and built a robust predictive model to identify key factors influencing real estate prices. The aim is to enable better decision-making in the real estate market.

---

## 🌟 **Key Features of the Project**
- **Comprehensive Exploratory Data Analysis (EDA):** Distribution analysis, correlation heatmaps, and outlier detection.
- **Feature Engineering:** Extracted `year_sold` and `month_sold` from the date column and identified the most important predictors.
- **Model Development:** Tested multiple regression models (e.g., Linear Regression, Decision Trees, LightGBM) and tuned hyperparameters for the best performance.
- **Final Model:** Achieved excellent results with **LightGBM Regressor**, ensuring minimal overfitting and high predictive power.

---

## 📊 **Dataset Overview**
The dataset contains **21,613 rows** and the following key columns:

| Column            | Description                                         |
|--------------------|-----------------------------------------------------|
| `id`              | Unique identifier for each property                 |
| `date`            | Date when the house was sold                        |
| `price`           | Sale price (target variable)                        |
| `bedrooms`        | Number of bedrooms                                  |
| `bathrooms`       | Number of bathrooms                                 |
| `sqft_living`     | Interior living space in square feet                |
| `sqft_lot`        | Land space in square feet                           |
| `waterfront`      | Whether the property has a waterfront view          |
| `view`            | Number of times the property was viewed             |
| `zipcode`         | ZIP code of the property                            |

---

## 🚀 **Methodology**
### **1. Data Cleaning and Preparation**
- Removed duplicates and checked for missing values.
- Converted the `date` column into `year_sold` and `month_sold`.
- Scaled numerical features for better model performance.

### **2. Exploratory Data Analysis (EDA)**
- Visualized data distributions using histograms and box plots.
- Analyzed correlations to identify the most important features.
- Detected and analyzed outliers to understand their impact on the model.

### **3. Model Development**
- Tested several regression models:
  - **Linear Regression**
  - **Ridge and Lasso Regression**
  - **Decision Tree**
  - **Random Forest**
  - **LightGBM**
- Used **GridSearchCV** for hyperparameter tuning.
- Evaluated performance using metrics:
  - **R² (Coefficient of Determination)**
  - **RMSE (Root Mean Squared Error)**
  - **MAE (Mean Absolute Error)**

### **4. Final Results**
- The best-performing model is **LightGBM Regressor**, with:
  - **R² (Train):** 0.9379
  - **R² (Test):** 0.8919
  - **RMSE (Test):** $57,463

---

## 📈 **Feature Importance**
The following features were identified as the most important predictors for house prices:
1. `sqft_living`
2. `grade`
3. `waterfront`
4. `sqft_basement`

---

## 🛠️ **How to Run the Project**
1. Clone this repository:
   ```bash
   git clone https://github.com/migueleven/King-County-House-Price-Prediction.git
   cd house-price-prediction

## 🔍 **Insights**
- Properties with larger living spaces (`sqft_living`) and higher grades tend to have higher prices.
- Waterfront properties significantly increase house values.
- Temporal patterns reveal that prices peak during summer months.

---

## 🌟 **Next Steps**
- Validate the model on a larger, more recent dataset.
- Explore additional features such as neighborhood-specific trends.
- Develop a user-friendly dashboard for real-time price predictions.

---

## 💬 **Contact**
Feel free to reach out for any questions or collaborations:
- **Name:** Miguel Ángel
- **Email:** miguelchamizo10@gmail.com
- **GitHub:** https://github.com/migueleven

---
