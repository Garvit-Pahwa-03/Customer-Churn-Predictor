# 🔄 Customer Churn Predictor

A machine learning web application that predicts whether a telecom customer is likely to churn, built with scikit-learn and deployed via Streamlit.

## 🚀 Live Demo

> Add your Streamlit deployment link here

---

## 📌 Overview

Customer churn is a critical business problem in the telecom industry. This project trains a classification model on customer data and serves real-time predictions through an interactive web interface.

---

## 🧠 ML Pipeline

- **Dataset**: 1,000 customer records with features like Age, Gender, Tenure, Monthly Charges, Contract Type, Internet Service, and Tech Support
- **Preprocessing**: Handled missing values (InternetService column), label encoding for categorical features, and feature scaling with `StandardScaler`
- **Models Evaluated**: Logistic Regression, Support Vector Machine (SVM), Random Forest Classifier
- **Hyperparameter Tuning**: `GridSearchCV` with 5-fold cross-validation
- **Best Model**: SVM (via GridSearchCV) — **86% accuracy** on test set
- **Serialization**: Model and scaler saved with `joblib`

---

## 🖥️ App Features

- Input fields for Age, Gender, Tenure, and Monthly Charges
- Instant churn prediction (Yes / No) on button click
- Clean UI built with Streamlit

---

## 🗂️ Project Structure

```
├── app.py                  # Streamlit web app
├── notebook.ipynb          # EDA, model training & evaluation
├── model.pkl               # Trained SVM model
├── scaler.pkl              # Fitted StandardScaler
├── customer_churn_data.csv # Dataset
└── README.md
```

---

## ⚙️ Setup & Run Locally

```bash
# Clone the repo
git clone https://github.com/your-username/customer-churn-predictor.git
cd customer-churn-predictor

# Install dependencies
pip install streamlit scikit-learn numpy joblib pandas

# Run the app
streamlit run app.py
```

---

## 📊 Model Comparison

| Model | Accuracy |
|---|---|
| Logistic Regression | ~baseline |
| Random Forest (tuned) | 86% |
| **SVM (tuned) ✅** | **86%** |

---

## 🛠️ Tech Stack

`Python` `scikit-learn` `Streamlit` `pandas` `NumPy` `joblib`

---

## 📄 License

MIT License
