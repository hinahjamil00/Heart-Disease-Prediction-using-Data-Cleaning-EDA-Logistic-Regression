# ❤️ Heart Disease Prediction — Data Cleaning & Logistic Regression

This project focuses on **data preprocessing, exploratory data analysis (EDA), and machine learning modeling** to predict the presence of heart disease using patient medical attributes.

---

## 📌 Project Overview

The dataset contains medical information such as age, cholesterol level, chest pain type, blood pressure, and other clinical indicators. The goal is to build a classification model that predicts whether a patient has heart disease or not.

---

## 🎯 Target Variable

- **target**
  - `1` → Heart Disease Present  
  - `0` → No Heart Disease  

---

## 🧹 Data Cleaning Process

### ✔ Dataset Loading
- Loaded dataset using Pandas
- Checked structure, data types, and summary statistics

### ✔ Duplicate Handling
- Identified duplicate rows
- Removed duplicates to ensure data integrity

### ✔ Missing Value Treatment
- Checked for missing values
- No missing values found

### ✔ Outlier Treatment
- Applied **IQR method** to detect outliers
- Capped extreme values to reduce model distortion

### ✔ Feature Selection
- Removed low-variance or less informative features (e.g., `fbs`)
- Retained medically relevant predictors for modeling

---

## 📊 Exploratory Data Analysis (EDA)

### 📌 Target Distribution
- Analyzed class balance between 0 and 1

### 📌 Correlation Analysis
- Generated correlation heatmap
- Identified strong predictors:
  - `cp` (Chest Pain Type)
  - `thalach` (Max Heart Rate)
  - `oldpeak` (ST depression)
  - `ca` (number of vessels)
  - `exang` (exercise-induced angina)

### 📌 Feature Distributions
- Age distribution analysis
- Cholesterol distribution (including outliers)

### 📌 Feature vs Target Analysis
- Relationship between key features and heart disease outcome

---

## ⚙️ Feature Engineering & Preprocessing

- Applied **StandardScaler** for feature normalization
- Prepared dataset for machine learning models
- Split data into training and testing sets (80/20)

---

## 🤖 Machine Learning Model

### ✔ Logistic Regression

- Trained using scaled features
- Evaluated using test data
- Used as baseline classification model

---

## 📈 Model Evaluation

- Accuracy Score
- Precision, Recall, F1-score
- Confusion Matrix

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📂 Project Structure

```text
heart.csv
heart_data_loading_cleaning_logistic_regression.ipynb
README.md

## 👩‍💻 Author
Hina Jamil
