# 💳 Credit Card Fraud Detection

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning techniques.
The model classifies transactions as **fraudulent (1)** or **legitimate (0)**.

---

## 📂 Dataset

The dataset contains transaction details such as:

* Transaction amount (`amt`)
* Merchant and category
* Customer details (gender, location, etc.)
* Transaction time and location
* Target variable: `is_fraud`

Dataset used:

* `fraudTrain.csv`
* `fraudTest.csv`

---

## ⚙️ Technologies Used

* Python 🐍
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn

---

## 🔍 Steps Performed

### 1. Data Loading

* Loaded training and testing datasets
* Combined both datasets for preprocessing

### 2. Data Cleaning

* Removed unnecessary columns:

  * name, address, job, dob, etc.
* Checked for null values (none found)

### 3. Data Preprocessing

* Label Encoding for:

  * `merchant`
  * `category`
* One-Hot Encoding for categorical variables
* Feature scaling and imputation

### 4. Data Visualization

* Gender distribution plot
* Correlation heatmap

---

## 🤖 Models Used

### 1. Logistic Regression

* Accuracy: **~99%**
* Poor performance on fraud detection (imbalanced data issue)

### 2. Decision Tree

* Accuracy: **~99.6%**
* Better fraud detection compared to Logistic Regression

### 3. Random Forest ⭐

* Accuracy: **~99.7%**
* Best performing model
* Good balance between precision and recall

---

## 📊 Results

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 99.47%   |
| Decision Tree       | 99.62%   |
| Random Forest       | 99.73%   |

👉 Random Forest performed the best for fraud detection.

---

## ⚠️ Note

* Dataset is highly **imbalanced**
* Accuracy alone is not enough → precision & recall are important

---

## 🚀 Future Improvements

* Use SMOTE for balancing data
* Try advanced models (XGBoost, Neural Networks)
* Hyperparameter tuning

---

## 👩‍💻 Author

Sakshi

---
