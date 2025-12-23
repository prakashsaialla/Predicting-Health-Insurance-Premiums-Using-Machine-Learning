# Predicting Health Insurance Premiums Using Machine Learning

## 📌 Project Overview
This project focuses on predicting annual health insurance premiums using demographic and medical risk indicators.  
The objective is to help insurers estimate premiums more accurately while maintaining fairness and effective risk management.

---

## 🎯 Problem Statement
Health insurance pricing depends on multiple factors such as age, BMI, medical history, and lifestyle indicators.  
Traditional pricing methods struggle to capture nonlinear relationships and correlated medical variables.

**Key Questions Addressed:**
- Can machine learning accurately predict insurance premiums before underwriting?
- Which factors most strongly influence premium pricing?
- Which model performs best for this real-world healthcare dataset?

---

## 📊 Dataset Overview
- **Total Records:** 986  
- **Total Features:** 11  
- **Target Variable:** `PremiumPrice`  
- **Data Type:** Numeric (No missing values)

### Key Features
- Age  
- Height, Weight, BMI  
- Diabetes, Blood Pressure Problems  
- Chronic Diseases  
- Number of Major Surgeries  
- Family Medical History  

---

## 🔍 Exploratory Data Analysis (EDA)
- Premiums increase significantly with **age and BMI**
- Individuals with **chronic diseases, diabetes, BP issues, and surgical history** pay higher premiums
- Target variable showed **right skewness**, handled using **log transformation**
- Interaction between **age and BMI** showed strong combined risk effect

---

## 🧪 Data Preprocessing & Feature Engineering
- Verified data quality (no missing values)
- Applied **log transformation** on premium prices
- Created derived features:
  - BMI
  - BMI Category (Underweight, Normal, Overweight, Obese)
  - Age Groups
  - Weight–Height Ratio
- Encoded categorical variables using dummy variables

---

## 🤖 Modeling Approach
### Models Tried:
- Linear Regression
- OLS Regression with VIF
- Random Forest Regressor
- Gradient Boosting
- **XGBoost Regressor (Final Model)**

### Why XGBoost?
- Handles **multicollinearity**
- Captures **nonlinear relationships**
- Robust to correlated medical variables
- Prevents overfitting using regularization

---

## 📈 Model Performance
- **R² Score:** ~0.84  
- **MAE:** Low  
- **RMSE:** Low  
- **Cross-Validation:** Stable 5-fold results  
- No significant overfitting observed

---

## 💡 Business Impact
- Enables faster and more consistent underwriting
- Improves pricing fairness
- Helps identify high-risk customer segments
- Supports data-driven preventive healthcare strategies

---

## 🛠 Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🚀 Future Improvements
- Include lifestyle features (smoking, alcohol, activity level)
- Deploy model using Flask or FastAPI
- Build an interactive dashboard
- Test deep learning approaches

---

## 👥 Contributors
- Vineet Reddy Saddi  
- Shiva Kotagiri  
- Svamsee Addaguduru  
- Prakash Sai Alla  
- Saleeq Sunil  

---

⭐ If you found this project useful, feel free to star the repository!
