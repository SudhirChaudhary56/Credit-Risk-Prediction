# Credit-Risk-Prediction
# 🏦 Credit Risk Prediction – Machine Learning Project

Predicting whether a customer will default on their loan within the next 2 years using Kaggle's **Give Me Some Credit** dataset.

---

## 📘 Overview
This project builds a binary classification model to predict loan default risk.  
Used **Logistic Regression**, **Random Forest**, and **SHAP** explainability for a complete ML workflow.

---

## 🔄 Project Workflow
1. Data Loading  
2. Missing Value Handling  
3. Exploratory Data Analysis (EDA)  
4. Train-Test Split (Stratified)  
5. Feature Scaling (for LR)  
6. Model Training: Logistic Regression & Random Forest  
7. Evaluation (AUC, Recall, Confusion Matrix)  
8. SHAP Explainability  
9. Save Final Model (.pkl)

---

## 🗂️ Dataset Details
- **Source:** Kaggle – Give Me Some Credit  
- **Rows:** ~150,000  
- **Task:** Predict if customer defaults within 2 years  
- **Target:** `SeriousDlqin2yrs`  
- **Issue:** Highly imbalanced data  

---

## 🛠 Tech Stack
- Python  
- NumPy  
- Pandas  
- Matplotlib/Seaborn  
- Scikit-Learn  
- SHAP  
- Jupyter Notebook  

---

## 🤖 Modeling Approach

### 1️⃣ Logistic Regression
- Scaled features (StandardScaler)  
- Balanced class weights  
- Good baseline model  

### 2️⃣ Random Forest (Best Model)
- 200 trees  
- Handles imbalance  
- Captures non-linear patterns  

---

## 📊 Results

### ⭐ Best Model → Random Forest
- **AUC:** ~0.84  
- **Accuracy:** ~94%  
- **Recall (Defaults):** Improved using `class_weight='balanced'`  

---

## 🔍 Key Insights
- Dataset is highly imbalanced → stratified split + balanced weights used  
- Most important features:  
  1. RevolvingUtilizationOfUnsecuredLines  
  2. NumberOfTimes90DaysLate  
  3. DebtRatio  
  4. Age  
  5. NumberOfOpenCreditLinesAndLoans  
- Random Forest performed significantly better  
- SHAP helped explain feature contributions clearly  

---

## 🧠 SHAP Explainability
Used SHAP summary bar plot to interpret how each feature affects model predictions.  
This helps banks understand **why** a customer is predicted as risky.

---

## 📁 Project Files
- `credit_risk_project.ipynb` — Main Notebook  
- `requirements.txt` — Libraries  
- `reports/Credit_Risk_Project_Final_Report.pdf`  
- `reports/Credit_Risk_Project_Presentation.pptx`  
- `models/credit_risk_model.pkl`  

---

## 📂 Folder Structure

```
Credit-Risk-Prediction/
│
├── credit_risk_project.ipynb
├── README.md
├── requirements.txt
│
├── reports/
│   ├── Credit_Risk_Project_Final_Report.pdf
│   └── Credit_Risk_Project_Presentation.pptx
│
├── models/
│   └── credit_risk_model.pkl
```

---

## ▶️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Then open:

```
credit_risk_project.ipynb
```

---

## 💼 Business Impact
- Detect high-risk customers early  
- Reduce loan default losses  
- Improve financial decision-making  
- Enable faster loan approvals  

---

## 👤 Author
**Sudhir Chaudhary**  
Email: **sudhirchaudhary4565@gmail.com**  
GitHub: **https://github.com/SudhirChaudhary56**
