# Perceptron

<p align="center">
  <img src="https://miro.medium.com/0*Ib3_FfuOy04kOmfO" width="600"/>
</p>

---

## Overview

The **Perceptron** is one of the earliest and simplest types of **artificial neural networks**, used for **binary classification** tasks.

It models a decision boundary as a **linear function** and classifies inputs into two categories based on whether they fall on one side of the boundary or the other.

---

## Objective

- Perform binary classification  
- Learn a linear decision boundary  
- Understand foundational neural network concepts  
- Serve as a building block for more complex models  

---

## What is a Perceptron?

A Perceptron takes multiple input features, applies weights, and produces an output based on a threshold.

In simple terms:  
It decides whether a data point belongs to one class or another using a linear rule.

---

## How It Works

1. Initialize weights and bias  
2. Compute weighted sum of inputs  
3. Apply activation function  
4. Generate prediction  
5. Update weights if prediction is incorrect  
6. Repeat until convergence  

---

## Model Representation

- Input features mapped to weighted sum  
- Linear decision boundary (hyperplane)  
- Binary output (0 or 1)  

---

## Formulas

### Linear Combination

z = wᵀx + b  

---

### Activation Function (Step Function)

ŷ = 1, if z ≥ 0  
ŷ = 0, if z < 0  

---

### Weight Update Rule

w = w + α · y · x  

b = b + α · y  

Where:  
- w → Weight vector  
- x → Input vector  
- b → Bias  
- α → Learning rate  
- y → True label  

---

## Methodology

- Compute prediction using linear combination  
- Compare prediction with actual label  
- Update weights if misclassified  
- Iterate until classification improves  

---

## Key Concepts

- Linear separability assumption  
- Binary classification  
- Decision boundary (hyperplane)  
- Online learning (updates per sample)  

---

## Advantages

- Simple and easy to implement  
- Fast training  
- Works well for linearly separable data  
- Interpretable model  

---

## Limitations

- Only works for linearly separable data  
- Cannot solve non-linear problems (e.g., XOR)  
- Sensitive to noisy data  
- Limited expressive power  

---

## Applications

- Binary classification problems  
- Spam detection  
- Sentiment classification  
- Basic pattern recognition  

---

## References

- https://scikit-learn.org/stable/modules/linear_model.html#perceptron  
- https://www.deeplearningbook.org/  
- https://developers.google.com/machine-learning/crash-course  
- https://www.ibm.com/topics/perceptron  
- https://en.wikipedia.org/wiki/Perceptron  

---
