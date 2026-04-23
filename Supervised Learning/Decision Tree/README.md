# Decision Trees

<p align="center">
  <img src="https://www.cfoselections.com/hubfs/when%20to%20use%20a%20decision%20tree%20for%20business%20planning.png" width="600"/>
</p>

# Decision Trees

## Overview

Decision Trees are a non-parametric supervised learning method used for both classification and regression tasks. They model decision-making processes using a hierarchical, tree-like structure, where each internal node represents a feature-based condition, each branch represents an outcome, and each leaf node represents a final prediction.

They are widely used due to their interpretability, ability to capture non-linear relationships, and minimal preprocessing requirements.

---

## Learning Objectives

- Understand the structure and working of decision trees  
- Learn how splitting decisions are made using impurity measures  
- Analyze strengths and limitations of tree-based models  
- Build intuition for model tuning and optimization  

---

## Problem Formulation

Given input features \( X \) and target variable \( y \), the objective is to learn a function:

f(X) → y  

The model partitions the feature space into regions and assigns predictions based on the majority class (classification) or mean value (regression) within each region.

---

## How Decision Trees Work

Decision Trees recursively split the dataset into subsets based on feature values.

At each node:
- A feature is selected  
- A threshold or condition is applied  
- The dataset is divided into subsets  
- The process continues recursively  

Each path from root to leaf represents a decision rule.

---

## Splitting Criteria

### Classification

**Gini Impurity**  
Measures the probability of incorrect classification:

Gini = 1 − Σ (pᵢ)²  

**Entropy**  
Measures randomness or disorder:

Entropy = − Σ pᵢ log₂(pᵢ)  

The algorithm selects splits that minimize impurity.

---

### Regression

**Mean Squared Error (MSE)**  
Measures variance within a node and is minimized during splitting.

---

## Algorithm Workflow

1. Start with the full dataset as the root node  
2. Evaluate all possible splits across features  
3. Select the split that maximizes information gain or minimizes error  
4. Partition the dataset  
5. Repeat recursively for each subset  
6. Stop when:
   - Maximum depth is reached  
   - Minimum samples per node is reached  
   - No further improvement is possible  

---

## Model Complexity and Overfitting

Decision Trees tend to overfit when allowed to grow deep. Controlling complexity is critical.

### Common Regularization Techniques

- Max depth restriction  
- Minimum samples per split  
- Minimum samples per leaf  
- Pruning (pre-pruning and post-pruning)  

---

## Advantages

- Highly interpretable and easy to visualize  
- Handles both numerical and categorical data  
- Requires minimal feature scaling  
- Captures non-linear relationships  
- Fast inference time  

---

## Limitations

- Prone to overfitting  
- Sensitive to small changes in data  
- Can become unstable with noisy data  
- Bias toward features with more splits  

---

## Improving Performance

- Use pruning to simplify trees  
- Apply cross-validation for model selection  
- Normalize or preprocess data where required  
- Use ensemble methods:
  - Random Forest  
  - Gradient Boosting  

---

## Applications

Decision Trees are widely used in:

- Fraud detection  
- Medical diagnosis  
- Credit risk modeling  
- Customer segmentation  
- Recommendation systems  
- Business decision analysis  

---

## Implementation in This Repository

This module includes:

- Decision tree implementations  
- Experiments with different splitting criteria  
- Analysis of model performance  
- Exploration of overfitting vs generalization  

---

## Evaluation Metrics

### Classification

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

### Regression

- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

---

## Key Takeaways

- Decision Trees break complex problems into simple decision rules  
- They are powerful baseline models for many tasks  
- Model performance depends on proper regularization  
- They form the foundation for ensemble learning techniques  

---

## Conclusion

Decision Trees provide a balance between interpretability and predictive capability. While simple in structure, they are highly effective and form the basis of advanced models such as Random Forests and Gradient Boosting, which are widely used in production systems.l-world strategic decision-making scenarios.
