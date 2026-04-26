# Ensemble Learning: Regression and Classification

<div align="center">
  <img src="https://www.ibm.com/adobe/dynamicmedia/deliver/dm-aid--fc4f06fb-b27c-424b-9180-3163e7d2825e/ensemble-learning-boosting.png" width="700"/>
</div>

---

## Overview

This project demonstrates practical implementations of ensemble learning techniques for both regression and classification problems. It also establishes the theoretical foundation using decision trees, which serve as the base learners for most ensemble methods.

Ensemble learning improves accuracy, robustness, and generalization by combining multiple models, while decision trees provide the underlying structure for learning complex decision boundaries.

---

## Decision Trees

<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f3/CART_tree_titanic_survivors.png/800px-CART_tree_titanic_survivors.png" width="600"/>
</div>

### Overview

Decision Trees are a non-parametric supervised learning method used for both classification and regression tasks. They model decision-making processes using a hierarchical tree structure.

Each internal node represents a feature-based condition, each branch represents an outcome, and each leaf node represents a final prediction.

---

### Learning Objectives

- Understand tree structure and recursive splitting  
- Learn impurity-based decision making  
- Analyze strengths and limitations  
- Build intuition for model tuning  

---

### Problem Formulation

Given input features \( X \) and target variable \( y \), the objective is to learn a function:

f(X) → y  

The model partitions the feature space into regions and assigns predictions based on majority class (classification) or mean value (regression).

---

### How Decision Trees Work

- Select best feature and threshold  
- Split dataset into subsets  
- Recursively repeat splitting  
- Continue until stopping criteria are met  

Each root-to-leaf path represents a decision rule.

---

### Splitting Criteria

#### Classification

Gini Impurity  
Gini = 1 − Σ (pᵢ)²  

Entropy  
Entropy = − Σ pᵢ log₂(pᵢ)  

#### Regression

Mean Squared Error (MSE)

---

### Algorithm Workflow

1. Start with full dataset  
2. Evaluate all splits  
3. Choose best split  
4. Partition data  
5. Repeat recursively  
6. Stop based on constraints  

---

### Model Complexity and Overfitting

Decision trees tend to overfit when deep.

#### Regularization Techniques

- Max depth  
- Minimum samples per split  
- Minimum samples per leaf  
- Pruning  

---

### Advantages

- Interpretable  
- Handles non-linearity  
- Minimal preprocessing  
- Works with mixed data types  

---

### Limitations

- Overfitting  
- Instability  
- Sensitive to noise  
- Biased toward dominant features  

---

## Ensemble Learning

### Key Concepts

- Bagging reduces variance  
- Boosting reduces bias  
- Stacking combines models using meta-learning  

---

## Why Ensemble Learning Builds on Trees

Decision Trees are high-variance models. Ensemble methods improve them by:

| Method        | Improvement Mechanism |
|--------------|----------------------|
| Bagging      | Reduces variance     |
| Boosting     | Reduces bias         |
| Stacking     | Improves prediction  |

---

## Project Files

- `CODE Regressor.ipynb` — Ensemble models for regression  
- `CODE Classification.ipynb` — Ensemble models for classification  

---

## Regression Implementation

### Models Used

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Gradient Boosting Regressor  

### Metrics

- RMSE  
- R² Score  

---

## Classification Implementation

### Models Used

- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  
- AdaBoost / Gradient Boosting  
- Voting Classifier  

### Metrics

- Accuracy  
- Precision  
- Recall  
- Confusion Matrix  

---

## Workflow

1. Data loading  
2. Preprocessing  
3. Baseline modeling  
4. Ensemble application  
5. Evaluation  

---

## Improving Performance

- Hyperparameter tuning  
- Cross-validation  
- Feature engineering  
- Ensemble selection  

---

## Applications

- Fraud detection  
- Medical diagnosis  
- Credit scoring  
- Customer segmentation  
- Recommendation systems  

---

## Technology Stack

- Python  
- Scikit-learn  
- Pandas, NumPy  
- Matplotlib  

---

## How to Run

```bash
pip install numpy pandas scikit-learn matplotlib
jupyter notebook
