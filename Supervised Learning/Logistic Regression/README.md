# Logistic Regression

<p align="center">
  <img src="https://media.licdn.com/dms/image/v2/D4D12AQFQ7aHxzmUiGQ/article-cover_image-shrink_600_2000/article-cover_image-shrink_600_2000/0/1673330159582?e=2147483647&v=beta&t=pwyWZwEXt3yMubRe40aZkR-IluJVp5aGM-2gjGO0SWg" width="600"/>
</p>

---

## Overview

**Logistic Regression** is a supervised machine learning algorithm used for **classification problems**, particularly when the target variable is binary (0/1).

Instead of predicting continuous values, it estimates the **probability of an event occurring**, using a transformation that ensures outputs lie between 0 and 1. :contentReference[oaicite:0]{index=0}

---

## Objective

- Model probability of categorical outcomes  
- Perform binary and multi-class classification  
- Estimate relationships between features and class labels  
- Provide interpretable probabilistic predictions  

---

## What is Logistic Regression?

Logistic Regression predicts the **probability of a class label** based on input features.

In simple terms:  
It transforms a linear equation into a probability using an S-shaped (sigmoid) curve.

---

## How It Works

1. Compute a linear combination of input features  
2. Apply a sigmoid (logistic) function  
3. Convert output into probability (0 to 1)  
4. Apply threshold (e.g., 0.5) for classification  
5. Optimize parameters using likelihood-based methods  

---

## Model Representation

- Binary classification (most common)  
- Multinomial logistic regression (multi-class)  
- Extension of linear regression for classification tasks  

---

## Formulas

### Linear Model

z = β₀ + β₁x₁ + β₂x₂ + ... + βₙxₙ  

---

### Sigmoid (Logistic Function)

p = 1 / (1 + e^(−z))  

This maps any real value to a probability between 0 and 1. :contentReference[oaicite:1]{index=1}  

---

### Log-Odds (Logit Function)

log(p / (1 − p)) = β₀ + β₁x₁ + ... + βₙxₙ  

Logistic regression models **log-odds as a linear function of inputs**. :contentReference[oaicite:2]{index=2}  

---

### Cost Function (Log Loss / Cross-Entropy)

J = −(1/n) Σ [yᵢ log(pᵢ) + (1 − yᵢ) log(1 − pᵢ)]  

---

### Gradient Descent Update

w = w − α · ∇J(w)  
b = b − α · ∂J/∂b  

---

## Methodology

- Compute linear predictor  
- Apply sigmoid transformation  
- Estimate probability of class membership  
- Optimize parameters using Maximum Likelihood Estimation (MLE)  
- Classify based on probability threshold  

---

## Key Concepts

- Probability vs log-odds  
- Sigmoid function (S-shaped curve)  
- Threshold-based classification  
- Maximum Likelihood Estimation  
- Odds and odds ratio interpretation  

---

## Advantages

- Interpretable and probabilistic output  
- Efficient and fast to train  
- Works well for linearly separable classes  
- Strong baseline classification model  

---

## Limitations

- Assumes linear decision boundary  
- Sensitive to outliers  
- Cannot capture complex non-linear patterns  
- Performance depends on feature engineering  

---

## Applications

- Credit risk prediction  
- Medical diagnosis (disease vs no disease)  
- Spam detection  
- Customer churn prediction  
- Fraud detection  

---

## References

- https://scikit-learn.org/stable/modules/linear_model.html#logistic-regression  
- https://developers.google.com/machine-learning/crash-course/classification/logistic-regression  
- https://www.statlearning.com/  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  
- https://www.ibm.com/topics/logistic-regression  

---
