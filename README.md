# loan-prediction

Here's a well-structured README for your **Loan Prediction** project:

---

# 📌 Loan Prediction Project

## 📖 Introduction

This is a **loan prediction system** built using **Python** and **machine learning algorithms**. The goal is to classify loan applications as **approved (Y) or not approved (N)** based on multiple financial and demographic factors.

We explored **logistic regression, decision trees, and random forests**, compared their performance, and optimized hyperparameters using **GridSearchCV**.

---

## 🎯 Problem Statement

The objective is to **predict whether a loan will be approved** based on factors such as **applicant income, loan amount, credit history, and more**. This is a **binary classification problem** where we predict one of two outcomes:  
✔ **Approved (Y)**  
✖ **Not Approved (N)**

---

## 📊 Dataset

The dataset consists of **614 training samples** and **367 test samples** with the following features:

| Feature Name        | Type        | Description                                  |
| ------------------- | ----------- | -------------------------------------------- |
| `Loan_ID`           | Numerical   | Unique identifier for the loan               |
| `Gender`            | Categorical | Male / Female                                |
| `Married`           | Categorical | Applicant married (Yes/No)                   |
| `Dependents`        | Categorical | Number of dependents (0, 1, 2, 3+)           |
| `Education`         | Categorical | Graduate / Non-Graduate                      |
| `Self_Employed`     | Categorical | Self-employed (Yes/No)                       |
| `ApplicantIncome`   | Numerical   | Applicant's income                           |
| `CoapplicantIncome` | Numerical   | Co-applicant's income                        |
| `LoanAmount`        | Numerical   | Loan amount requested (in thousands)         |
| `Loan_Amount_Term`  | Numerical   | Loan repayment period (months)               |
| `Credit_History`    | Categorical | Past credit history (1 = good, 0 = bad)      |
| `Property_Area`     | Categorical | Urban / Semi-Urban / Rural                   |
| `Loan_Status`       | Categorical | Target variable (Y = Approved, N = Rejected) |

---

## 🔍 Approach

1️⃣ **Exploratory Data Analysis (EDA)** → Understanding the dataset, visualizing correlations  
2️⃣ **Data Preprocessing** → Handling missing values, encoding categorical variables  
3️⃣ **Feature Engineering** → Creating new meaningful features like **Total Income** & **EMI**  
4️⃣ **Model Development** → Training machine learning models  
5️⃣ **Evaluation & Optimization** → Comparing models and using hyperparameter tuning

---

## 🏆 Models & Performance

We implemented three models and compared their validation accuracy:

| Model                   | Mean Validation Accuracy |
| ----------------------- | ------------------------ |
| **Logistic Regression** | **80.3%** ✅             |
| Random Forest           | 78.3%                    |
| Decision Tree           | 71.1%                    |

- **Logistic Regression performed the best** due to its simplicity and effectiveness.
- **Hyperparameter tuning using GridSearchCV** improved Random Forest accuracy from 78.3% to **81.3%**.

---

## 📈 Data Visualization

We used **heatmaps**, **pair plots**, and **correlation matrices** to explore relationships between variables.

✅ Higher **Applicant Income** correlates with loan approval.  
✅ Good **Credit History** significantly increases approval chances.  
✅ Smaller **Loan Amount** improves approval probability.

---

## 🚀 Future Improvements

🔹 Try **ensemble learning** (stacking multiple models)  
🔹 Add more **domain-specific features**  
🔹 Use **Neural Networks (TensorFlow/PyTorch)** for better accuracy

---

## 🛠️ Technologies Used

- **Python** 🐍
- **Scikit-Learn** (Machine Learning)
- **Pandas & NumPy** (Data Handling)
- **Matplotlib & Seaborn** (Visualization)

---

## 📌 How to Run

1️⃣ Clone the repository

```bash
git clone https://github.com/MohdSafiya02/loan-prediction.git
cd loan-prediction
```

2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

3️⃣ Run the model

```bash
python loan_prediction.py
```

---
