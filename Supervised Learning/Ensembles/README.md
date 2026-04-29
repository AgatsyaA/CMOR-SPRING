# Ensemble Learning: Regression and Classification

<div align="center">
  <img src="https://www.ibm.com/adobe/dynamicmedia/deliver/dm-aid--fc4f06fb-b27c-424b-9180-3163e7d2825e/ensemble-learning-boosting.png" width="700"/>
</div>

---

## Overview

**Ensemble Learning** is a machine learning paradigm that combines multiple models to improve **accuracy, robustness, and generalization**.

Instead of relying on a single model, ensemble methods aggregate predictions from multiple learners to produce a more reliable output.

---

## Objective

- Improve prediction accuracy  
- Reduce variance and bias  
- Enhance model stability  
- Combine strengths of multiple models  

---

## What is Ensemble Learning?

Ensemble learning combines multiple base models to produce a final prediction.

In simple terms:  
Many weak learners come together to form a strong learner.

---

## Types of Ensemble Methods

### Bagging (Bootstrap Aggregating)

- Trains multiple models on **random subsets of data**  
- Reduces **variance**  
- Models trained independently  

**Example:** Random Forest  

---

### Boosting

- Trains models **sequentially**  
- Focuses on correcting previous errors  
- Reduces **bias and variance**  

**Examples:** AdaBoost, Gradient Boosting  

---

### Stacking

- Combines multiple models using a **meta-learner**  
- Learns how to best combine predictions  

---

## How It Works

1. Train multiple base learners  
2. Combine predictions:
   - Averaging (regression)  
   - Voting (classification)  
3. Generate final prediction  

---

## Formulas

### Bagging (Averaging for Regression)

ŷ = (1/M) Σ ŷᵢ  

Where:  
- M → Number of models  

---

### Voting (Classification)

ŷ = mode(ŷ₁, ŷ₂, ..., ŷₘ)  

---

### Boosting (General Form)

F(x) = Σ αₘ hₘ(x)  

Where:  
- hₘ(x) → Weak learner  
- αₘ → Weight assigned to learner  

---

### Gradient Boosting Update

Fₘ(x) = Fₘ₋₁(x) + γₘ hₘ(x)  

---

## Key Concepts

- Weak vs strong learners  
- Bias-variance tradeoff  
- Model diversity  
- Sequential vs parallel learning  

---

## Advantages

- Improves accuracy significantly  
- Reduces overfitting  
- Works well on complex datasets  
- Robust to noise (depending on method)  

---

## Limitations

- Increased computational cost  
- Less interpretable than single models  
- Requires careful tuning  
- Risk of overfitting in boosting  

---

## Regression Implementation

### Models Used

- Linear Regression  
- Random Forest Regressor  
- Gradient Boosting Regressor  

### Metrics

- RMSE  
- R² Score  

---

## Classification Implementation

### Models Used

- Logistic Regression  
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

1. Data preprocessing  
2. Baseline modeling  
3. Ensemble model training  
4. Performance evaluation  
5. Model comparison  

---

## Improving Performance

- Hyperparameter tuning  
- Cross-validation  
- Feature engineering  
- Model selection and stacking  

---

## Applications

- Fraud detection  
- Medical diagnosis  
- Credit scoring  
- Recommendation systems  
- Customer segmentation  

---

## Implementation in This Repository

- Ensemble models for regression and classification  
- Comparison with baseline models  
- Performance evaluation and tuning  

---

## Repository Structure

Ensembles/

├── regression models  
├── classification models  
└── README.md  

---

## Key Takeaways

- Ensemble methods combine multiple models to improve performance  
- Bagging reduces variance, Boosting reduces bias  
- Stacking learns optimal model combinations  
- Widely used in real-world ML systems  

---

## References

- https://scikit-learn.org/stable/modules/ensemble.html  
- https://developers.google.com/machine-learning/crash-course  
- https://www.statlearning.com/  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  
- https://www.ibm.com/topics/ensemble-learning  

---
