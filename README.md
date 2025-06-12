# Customer-Churn-Prediction
 Predicting  which customers are likely to stop using a service.
# 📊 Customer Churn Prediction using Machine Learning

This project is a supervised machine learning analysis to predict customer churn in a telecom company. It involves data preprocessing, model training, evaluation, and visualization using Python libraries like pandas, scikit-learn, XGBoost, seaborn, and matplotlib.

---

## 📁 Dataset

- **Name:** Telco Customer Churn
- **Source:** [Kaggle - IBM Sample Dataset](https://www.kaggle.com/blastchar/telco-customer-churn)
- **Format:** CSV
- **Records:** 7,043 customer entries
- **Target Variable:** `Churn` (Yes/No)

---

## 🛠 Features in Dataset

- **Customer Info:** customerID, gender, SeniorCitizen, Partner, Dependents
- **Services Signed Up:** PhoneService, MultipleLines, InternetService, OnlineSecurity, etc.
- **Account Info:** tenure, MonthlyCharges, TotalCharges
- **Target:** Churn (Yes/No)

---

## 📌 Objective

To build and evaluate machine learning models that predict whether a customer will churn (leave the company) based on their usage patterns and account information.

---

## 🔍 Project Workflow

### 1. **Data Preprocessing**
- Dropped `customerID` (not useful for prediction)
- Converted `TotalCharges` to numeric (and handled missing values)
- Encoded binary categorical columns using label mapping
- One-hot encoded multi-category categorical features
- Scaled features using `StandardScaler`

### 2. **Model Building**
We used and compared the following classifiers:
- Logistic Regression
- Random Forest
- XGBoost

### 3. **Model Evaluation**
Each model was evaluated using:
- Accuracy
- Recall (to capture actual churns)
- ROC-AUC Score
- ROC Curve Visualization

---

## 📊 Visualizations

- Count plot of churn distribution
- Correlation heatmap of features with `Churn`
- ROC curves for all models

---

## 💻 Technologies Used

- **Python 3.9+**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **XGBoost**
- **Jupyter Notebook**

---

## 🧠 How to Run the Project

1. Clone the repository or download the notebook.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost


---
## 🧠 How to Run Jupyter Notebook:
```bash
jupyter notebook
