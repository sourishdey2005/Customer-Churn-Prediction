# 📊 Customer Churn Prediction using Machine Learning

**Objective**: Predict which telecom customers are likely to stop using the service (churn) using supervised machine learning techniques like Logistic Regression, Random Forest, and XGBoost.

---

## 📁 Dataset Overview

- **Dataset Name**: Telco Customer Churn  
- **Source**: [Kaggle - IBM Sample Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)  
- **Format**: CSV  
- **Total Records**: 7,043 customer entries  
- **Target Variable**: `Churn` (Yes = Customer left, No = Customer stayed)

---

## 🛠 Features in the Dataset

- **Customer Demographics**:  
  - `customerID`, `gender`, `SeniorCitizen`, `Partner`, `Dependents`
- **Services Signed Up**:  
  - `PhoneService`, `MultipleLines`, `InternetService`, `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`, `StreamingTV`, `StreamingMovies`
- **Account Information**:  
  - `tenure`, `MonthlyCharges`, `TotalCharges`
- **Billing Preferences**:  
  - `PaperlessBilling`, `PaymentMethod`
- **Target**:  
  - `Churn` (Yes/No)

---

## 🎯 Project Goals

- Clean and preprocess the data for modeling
- Encode categorical and binary features properly
- Train and compare different machine learning models
- Evaluate models using performance metrics and plots
- Visualize churn-related insights

---

## 🔄 Project Workflow

### 📌 1. Data Preprocessing
- Removed `customerID` (not relevant for modeling)
- Converted `TotalCharges` to numeric (with missing values handled using mean imputation)
- Encoded binary columns (`Yes`/`No`) to `1`/`0`
- One-hot encoded multi-class categorical features (e.g., `InternetService`, `PaymentMethod`)
- Standardized the feature set using `StandardScaler`

### 🧠 2. Model Training
Trained and evaluated the following models:
- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

### 📏 3. Model Evaluation Metrics
Each model was evaluated using:
- **Accuracy** – Overall correctness of the model
- **Recall** – How many actual churns were correctly predicted
- **ROC-AUC Score** – Ability of the model to distinguish between churned and non-churned
- **ROC Curve** – Visualization of true positive vs. false positive rates

---

## 📊 Visualizations

- 📉 **Churn Distribution**: Bar chart of churn vs non-churn customers  
- 🔥 **Feature Correlation Heatmap**: Correlation between churn and other variables  
- 📈 **ROC Curves**: Comparison of all model performances  

---

## 🧰 Technologies Used

- **Language**: Python 3.9+
- **IDE**: Jupyter Notebook  
- **Libraries**:
  - `pandas`, `numpy` – Data manipulation  
  - `matplotlib`, `seaborn` – Data visualization  
  - `scikit-learn` – ML model building  
  - `xgboost` – Advanced boosting classifier  

---
