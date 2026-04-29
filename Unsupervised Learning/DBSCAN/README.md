# DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

<p align="center">
  <img src="https://ik.imagekit.io/upgrad1/abroad-images/imageCompo/images/img_0_1_86GN1D.png" width="600"/>
</p>

---

## Overview

**DBSCAN** is a density-based unsupervised learning algorithm used to cluster data points based on **density connectivity**. It groups points that are closely packed together while identifying points in low-density regions as **noise (outliers)**.

Unlike centroid-based methods such as K-Means, DBSCAN does not require specifying the number of clusters in advance and can detect clusters of **arbitrary shapes**.

---

## Learning Objectives

- Understand density-based clustering principles  
- Learn how DBSCAN identifies clusters and outliers  
- Analyze the impact of ε (epsilon) and MinPts  
- Evaluate clustering performance and limitations  

---

## Problem Formulation

Given a dataset X:

X = {x₁, x₂, ..., xₙ}

The objective is to group points into clusters such that:
- Points in the same cluster are **densely connected**
- Sparse regions are treated as **noise**

---

## Key Concepts

### Core Points
A point is a core point if it has at least **MinPts neighbors within radius ε**.

### Border Points
Points within the ε-neighborhood of a core point but not dense enough to be core points.

### Noise Points (Outliers)
Points that are neither core nor border points.

### Density Reachability
A point is directly reachable from another if it lies within ε and the source is a core point.

### Density Connectivity
Two points are connected if there exists a chain of core points linking them.

---

## Parameters

### Epsilon (ε)
Defines the neighborhood radius.

### MinPts
Minimum number of points required to form a dense region.

Proper selection of these parameters is critical for performance.

---

## Algorithm Workflow

1. Select an unvisited point  
2. Retrieve neighbors within ε  
3. If neighbors ≥ MinPts:
   - Mark as core point  
   - Create a new cluster  
   - Expand cluster using density reachability  
4. Else:
   - Mark as noise (may later become border)  
5. Repeat until all points are processed  

---

## Distance Metrics

- Euclidean Distance  
- Manhattan Distance  
- Cosine Distance  

Choice of metric significantly affects clustering behavior.

---

## Formulas

### Neighborhood Definition

Nε(x) = {y ∈ X | d(x, y) ≤ ε}

---

### Core Point Condition

|Nε(x)| ≥ MinPts

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

## Advantages

- No need to specify number of clusters  
- Detects clusters of arbitrary shape  
- Robust to noise and outliers  
- Effective for spatial data  

---

## Limitations

- Sensitive to ε and MinPts  
- Struggles with varying density clusters  
- Performance degrades in high dimensions  
- Distance metric impacts results  

---

## Parameter Selection Strategy

- Use **k-distance graph** to estimate ε  
- Set MinPts ≈ dimensions + 1  
- Apply feature scaling before clustering  

---

## Applications

- Anomaly detection  
- Geospatial clustering  
- Customer segmentation  
- Image processing  
- Fraud detection  

---

## Evaluation Techniques

- Silhouette Score  
- Visual inspection  
- Cluster density analysis  
- Domain-specific validation  

---

## Practical Considerations

- Feature scaling is essential  
- High dimensionality reduces effectiveness  
- PCA can improve clustering quality  
- Noise handling is a key advantage  

---

## Implementation in This Repository

- DBSCAN implementation  
- Parameter tuning experiments  
- Cluster and noise visualization  
- Comparison with other clustering methods  

---

## Repository Structure

DBSCAN/

├── implementation notebooks  
├── experiments  
└── README.md  

---

## Key Takeaways

- Clusters are formed based on **density, not centroids**  
- Automatically detects **outliers**  
- Works well for **irregular cluster shapes**  
- Requires careful parameter tuning  

---

## References

- https://scikit-learn.org/stable/modules/clustering.html#dbscan  
- https://developers.google.com/machine-learning/clustering/dbscan  
- https://www.statlearning.com/  
- https://link.springer.com/book/10.1007/978-0-387-84858-7  
- https://www.ibm.com/topics/dbscan  

---
