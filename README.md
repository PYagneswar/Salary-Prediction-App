# 💼 Salary Prediction Using Machine Learning

A machine learning project that predicts the expected salary (CTC) for a job applicant based on their experience, education, certifications, and other features — built as part of an internship capstone project.

---

## 📌 Problem Statement

To ensure fairness in the recruitment process, Company X wants to automate salary estimation based on historical applicant data. This eliminates bias and ensures consistent salary offers for similar profiles.

---

## 🎯 Objective

Develop a robust machine learning model to:
- Predict *Expected CTC* for new applicants
- Minimize human judgment in the salary offer process
- Deploy the model using a *Streamlit web app*

---

## 🧠 Project Phases

### ✅ Phase 1: Data Cleaning & EDA
- Removed rows with missing values
- Explored key trends using visualizations
- Saved correlation heatmap for reporting

### ✅ Phase 2: Feature Engineering & Model Training
- One-hot encoding for categorical variables
- Trained and evaluated:
  - Linear Regression
  - Random Forest
  - XGBoost
- Selected the *best model (XGBoost)* with R² ≈ 0.9998
- Saved trained model (salary_model.pkl) and feature list (model_features.pkl)

### ✅ Phase 3: Streamlit App
- Built a simple UI for real-time predictions
- Takes user inputs and displays predicted salary
- Uses the trained model for backend predictions

---

## 🗃 Dataset

- Provided as expected_ctc.csv
- Cleaned version saved as cleaned_expected_ctc.csv
- Contains features like:
  - Experience
  - Education level
  - Certifications
  - Publications
  - Current CTC
  - Preferred location, degree, and more

---

## 📊 Model Performance

| Model             | R² Score | RMSE (₹)     |
|-------------------|----------|--------------|
| Linear Regression | 0.9967   | ₹66,117.66   |
| Random Forest     | 0.9996   | ₹23,568.88   |
| XGBoost           | *0.9998* | *₹16,243.41* |

✅ *XGBoost* selected as the best model and used in the Streamlit app.

---

## 🚀 How to Run the Project

### 1. Clone this repository
```bash
git clone https://github.com/PYagneswar/salary-predictor.git
cd salary-predictor