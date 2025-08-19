# 🔗 Check Out My Other Project

**Also check my other repo from my GitHub profile: [ovm-studio](https://github.com/AnuragGupta181/ovm-studio)**  
A **frontend project** deployed at: **[ovm-studio.vercel.app](https://ovm-studio.vercel.app)**

# Loan Approval Prediction

## 📌 Objective
The goal of this project is to build a Machine Learning model that predicts whether a loan application will be approved or not, based on applicant details such as income, employment, education, property area, and credit history.  
This project is inspired by real-world banking scenarios where accurate predictions can improve decision-making and reduce risks.

---

## 📂 Dataset
- The dataset contains information about loan applicants including:
  - **ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term**
  - **Gender, Married, Dependents, Education, Self_Employed**
  - **Property_Area, Credit_History**
  - **Loan_Status** (Target: Approved = 1, Not Approved = 0)

---

## 🛠️ Steps Followed

### 1. Data Cleaning & Preprocessing
- Removed duplicates and irrelevant columns (e.g., Loan_ID).
- Handled missing values by filling with median/mode where appropriate.
- Converted categorical columns into numerical values:
  - Gender (Male=1, Female=0)
  - Education (Graduate=1, Not Graduate=0)
  - Property_Area (Rural=0, Semiurban=1, Urban=2), etc.
- Scaled numerical features (LoanAmount, ApplicantIncome, etc.).

### 2. Exploratory Data Analysis (EDA)
- Visualized **Loan Status distribution** (Approved vs Not Approved).
- Analyzed relationships:
  - Credit History strongly influences loan approval.
  - Semiurban applicants had higher approval rates.
  - Married and Male applicants showed slightly higher approvals.
- Correlation heatmap to understand feature relationships.

### 3. Model Building
Two classification models were trained:
- **Logistic Regression**
- **Decision Tree (criterion="entropy", max_depth=5)**

Data was split into **80% training, 20% testing** using stratified sampling.

### 4. Model Evaluation
- Metrics: **Accuracy, Confusion Matrix, Classification Report**
- Logistic Regression Accuracy: ~ (your notebook result, e.g. 81%)  
- Decision Tree Accuracy: ~ (your notebook result, e.g. 78%)  

📊 Logistic Regression performed slightly better, while Decision Tree provided interpretability.

---

## 📈 Results & Insights
- **Credit History** is the most important factor influencing loan approval.  
- Applicants from **Semiurban areas** had higher approval chances.  
- Income had some impact but was less significant than credit history.  
- Logistic Regression gave better accuracy, making it a good baseline model.  

---

## 🚀 Future Improvements (Optional)
- Use **Random Forest / XGBoost** for higher accuracy.
- Perform **hyperparameter tuning** for Decision Trees.
- Deploy as a **Streamlit web app** for real-time predictions.

---

## ✅ Conclusion
This project demonstrates the end-to-end ML workflow:
- Data cleaning and preprocessing
- Exploratory Data Analysis
- Model building and evaluation
- Insights for decision-making

Logistic Regression emerged as the better model, showing that simple linear models can often perform well in structured datasets.

---
