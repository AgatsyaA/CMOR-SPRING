# Unsupervised Learning

<p align="center">
  <img src="https://media.geeksforgeeks.org/wp-content/uploads/20251210102132756957/unsupervised_learning.webp" width="600"/>
</p>

---

## Overview

Unsupervised learning is a machine learning paradigm where models are trained on **unlabeled data** and must discover patterns, structures, or relationships without explicit guidance.

Unlike supervised learning, there are no predefined outputs. The model independently identifies meaningful groupings, representations, or anomalies within the data.

This module focuses on building a strong understanding of unsupervised techniques through practical implementations and analysis.

---

## Learning Objectives

- Understand how models learn from unlabeled data  
- Explore clustering and dimensionality reduction techniques  
- Analyze patterns and structures in datasets  
- Build intuition for exploratory data analysis  

---

## Problem Formulation

Given a dataset X without labels:

X = {x₁, x₂, ..., xₙ}

The objective is to discover hidden structure such as:
- Groups (clusters)  
- Patterns  
- Low-dimensional representations  

---

## Key Concepts

### Pattern Discovery
Identifying hidden relationships and structures in data.

### Clustering
Grouping similar data points based on feature similarity.

### Dimensionality Reduction
Reducing features while preserving essential information.

### Anomaly Detection
Identifying rare or unusual data points.

---

## Algorithms Implemented

### K-Means Clustering
- Partitions data into K clusters  
- Minimizes intra-cluster variance  
- Sensitive to initialization  

### DBSCAN
- Density-based clustering  
- Detects arbitrary-shaped clusters  
- Handles noise effectively  

### Principal Component Analysis (PCA)
- Reduces dimensionality  
- Captures maximum variance  
- Improves visualization and efficiency  

---

## Formulas

### K-Means Objective Function

J = Σ Σ ||xᵢ − μⱼ||²  

Minimizes the distance between points and their assigned cluster centers.

---

### Euclidean Distance

d(x, y) = √Σ (xᵢ − yᵢ)²  

---

### Silhouette Score

S = (b − a) / max(a, b)  

Where:  
- a → Mean intra-cluster distance  
- b → Mean nearest-cluster distance  

---

### PCA Transformation

Z = XW  

Where:  
- X → Data matrix  
- W → Eigenvectors (principal components)  
- Z → Transformed data  

---

## Repository Structure

Unsupervised Learning/

├── DBSCAN/  
├── K-Means/  
└── PCA/  

---

## Advantages

- No labeled data required  
- Useful for exploratory analysis  
- Identifies hidden patterns  
- Works well on large datasets  

---

## Limitations

- Hard to evaluate results  
- Sensitive to parameter selection  
- Requires interpretation  
- May produce ambiguous clusters  

---

## Applications

- Customer segmentation  
- Anomaly detection  
- Recommendation systems  
- Image compression  
- Feature extraction  

---

## Evaluation Techniques

- Silhouette Score  
- Elbow Method  
- Visual inspection  
- Reconstruction error (PCA)  

---

## References

- https://scikit-learn.org/stable/unsupervised_learning.html  
- https://developers.google.com/machine-learning/clustering  
- https://www.statlearning.com/  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  
- https://www.ibm.com/topics/unsupervised-learning  

---
