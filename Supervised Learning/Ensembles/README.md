<div align="center">
  <img src="https://miro.medium.com/v2/resize:fit:1400/1*7nZ4W9rj9xj9XK8J6X2s9A.png" width="700"/>
</div>

# 🤖 Ensemble Learning: Regression & Classification

---

## 📌 Overview

This project demonstrates practical implementations of **Ensemble Learning techniques** for both:

- 📈 Regression Problems  
- 🧠 Classification Problems  

Ensemble learning improves **accuracy, robustness, and generalization** by combining multiple models.

---

## 🧠 Key Concepts

- **Bagging (Bootstrap Aggregation)** → Reduces variance  
- **Boosting** → Reduces bias  
- **Stacking** → Combines multiple models using a meta-learner  

---

## 📂 Project Files

- `CODE Regressor.ipynb` → Ensemble models for regression  
- `CODE Classification.ipynb` → Ensemble models for classification  

---

## 📊 Regression (CODE Regressor.ipynb)

### 🔍 Implementations:
- Data preprocessing  
- Base models (Linear Regression, Decision Trees)  
- Ensemble models:
  - Random Forest Regressor  
  - Gradient Boosting Regressor  

### 📈 Metrics:
- RMSE  
- R² Score  

---

## 🧠 Classification (CODE Classification.ipynb)

### 🔍 Implementations:
- Data preprocessing  
- Base classifiers (Logistic Regression, Decision Tree)  
- Ensemble models:
  - Random Forest Classifier  
  - AdaBoost / Gradient Boosting  
  - Voting Classifier  

### 📊 Metrics:
- Accuracy  
- Precision / Recall  
- Confusion Matrix  

---

## ⚙️ Workflow

1. Load dataset  
2. Preprocess data  
3. Train baseline models  
4. Apply ensemble techniques  
5. Evaluate performance  

---

## 📈 Why Ensemble Learning?

| Problem            | Solution                |
|-------------------|------------------------|
| High Variance      | Bagging                |
| High Bias          | Boosting               |
| Model Limitations  | Stacking               |

---

## 🛠️ Tech Stack

- Python  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib  

---

## 🚀 How to Run

```bash
pip install numpy pandas scikit-learn matplotlib
jupyter notebook
