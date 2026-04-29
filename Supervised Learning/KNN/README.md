# K-Nearest Neighbors (KNN)

<p align="center">
  <img src="https://miro.medium.com/0*ItVKiyx2F3ZU8zV5" width="600"/>
</p>

---

## Overview

**K-Nearest Neighbors (KNN)** is a supervised machine learning algorithm used for **classification** and **regression**. It predicts outcomes based on the **similarity (distance)** between data points.

KNN is a **non-parametric, instance-based (lazy learning)** algorithm that does not build an explicit model during training. Instead, it stores the dataset and performs computation at prediction time.

---

## Objective

- Classify data points based on similarity  
- Use distance-based learning  
- Identify patterns in feature space  
- Enable accurate multi-class classification  

---

## What is KNN?

KNN classifies a data point based on its **nearest neighbors in feature space**.

In simple terms:  
A data point is assigned the class that is most common among its closest neighbors.

---

## How It Works

1. Choose the number of neighbors (k)  
2. Compute distance between the new point and all training points  
3. Select the k closest neighbors  
4. Apply:
   - Classification → Majority vote  
   - Regression → Average of neighbors  
5. Assign final prediction  

---

## Distance Metrics

### Euclidean Distance  
d(x, y) = √Σ (xᵢ − yᵢ)²  

### Manhattan Distance  
d(x, y) = Σ |xᵢ − yᵢ|  

### Minkowski Distance  
d(x, y) = (Σ |xᵢ − yᵢ|ᵖ)^(1/p)  

---

## Prediction Formulas

### Classification (Majority Voting)  
ŷ = mode(y₁, y₂, …, yₖ)  

### Regression (Averaging)  
ŷ = (1/k) Σ yᵢ  

### Weighted KNN (Optional)  
ŷ = (Σ wᵢ · yᵢ) / (Σ wᵢ)  
where wᵢ = 1 / d(x, xᵢ)  

## Methodology

- Classification by proximity (majority voting)  
- Regression via averaging  
- Lazy learning (no training phase)  
- Local approximation (uses nearby data points)  
- Pattern recognition through similarity  

---

## Key Concepts

- K value → Number of neighbors  
- Distance metric → Defines similarity  
- Feature scaling → Important for accuracy  
- Local decision making → Based on neighborhood  

---

## Choosing the Right K

- Small k → High variance, sensitive to noise  
- Large k → Low variance, may underfit  

Optimal k is typically selected using cross-validation.

---

## Key Idea

**Similar data points exist close to each other in feature space.**

---

## Advantages

- Simple and intuitive  
- No training phase required  
- Works well with small datasets  
- Supports multi-class classification  

---

## Limitations

- Computationally expensive during prediction  
- Sensitive to feature scaling  
- Performance depends on k  
- Affected by noise and outliers  

---

## Applications

- Recommendation systems  
- Image classification  
- Pattern recognition  
- Medical diagnosis  
- Fraud detection  

---

## Conclusion

KNN is a simple yet powerful algorithm based on **distance-driven similarity**. Its effectiveness depends heavily on **feature scaling**, **distance metric**, and **choice of k**.

---

## References

- https://zilliz.com/blog/k-nearest-neighbor-algorithm-for-machine-learning  
- https://www.xlstat.com/solutions/features/k-nearest-neighbors-knn  

---
