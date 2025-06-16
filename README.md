# 🛍️ Spent Amount Prediction

This project aims to predict the **Yearly Amount Spent** by customers based on their digital interaction behavior on an e-commerce platform. Using feature engineering, exploratory data analysis, and multiple regression techniques, we identify the key drivers influencing customer spending and build a predictive model.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [EDA & Data Preprocessing](#eda--data-preprocessing)
- [Feature Engineering & Selection](#feature-engineering--selection)
- [Model Building](#model-building)
- [Results & Evaluation](#results--evaluation)
- [Conclusion](#conclusion)
- [Technologies Used](#technologies-used)

---

## 📈 Project Overview

The objective is to analyze user data and build a regression model to predict **Yearly Amount Spent**. Insights from this model can help businesses personalize marketing strategies and understand customer behavior.

---

## 📊 Dataset Description

The dataset contains user metrics such as:

- `Avg. Session Length`: Average session duration on the website.
- `Time on App`: Time spent on the mobile app.
- `Time on Website`: Time spent on the website.
- `Length of Membership`: Duration of customer membership.
- `Yearly Amount Spent`: Target variable.

**Note:** Columns like `Email`, `Address`, and `Avatar` were removed during preprocessing.

---

## 🧹 EDA & Data Preprocessing

- Checked for missing values, duplicates, and data types.
- Visualized feature distributions and checked for skewness.
- Identified and treated outliers using the **IQR method**.
- Data cleaned and reduced from 500 to 476 rows after outlier removal.

---

## 🧠 Feature Engineering & Selection

- Removed non-predictive columns.
- Verified no multicollinearity using **Variance Inflation Factor (VIF)**.
- Selected important features using:
  - **Correlation with Target**
  - **Recursive Feature Elimination (RFE)**

**Final Selected Features:**
- `Avg. Session Length`
- `Time on App`
- `Length of Membership`

---

## 🤖 Model Building

- Data split into training and testing sets (80:20).
- Applied **StandardScaler** for normalization.
- Trained and evaluated the following models:
  - Linear Regression
  - Lasso Regression
  - Ridge Regression
  - ElasticNet Regression

---

## 📊 Results & Evaluation

- **ElasticNet** selected as final model to prevent overfitting.

### 🔧 Hyperparameter Tuning

Used **GridSearchCV** to tune ElasticNet parameters for optimal performance.

---

## ✅ Conclusion

- The final model accurately predicts customer spending using a few key behavior-based features.
- **Top predictors**:
  - `Length of Membership`
  - `Avg. Session Length`
  - `Time on App`
- The project demonstrates effective use of feature selection, preprocessing, and regression analysis.

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Statsmodels
- Streamlit

---

## 📁 Project Status

✅ Completed – Predictive model built and validated and deploy on the Streamlit.


## 🚀 Streamlit Deployment

The project is deployed as a web application using [**Streamlit**](https://spent-amount-predictor-11.streamlit.app/) 



**Gaurav Pandey**  
_Data Science Enthusiast | Open to Work_  
Feel free to connect on [LinkedIn](https://www.linkedin.com/in/gaurav-pandey-data-enthusiast) or reach out for collaborations!

