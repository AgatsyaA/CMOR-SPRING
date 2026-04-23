# K-Means Clustering

<p align="center">
  <img src="https://miro.medium.com/0*Hx4ndu6ffRy0TtdF.png" width="600"/>
</p>

## Overview

K-Means is a centroid-based unsupervised learning algorithm used to partition data into K distinct clusters. It assigns each data point to the cluster with the nearest centroid, with the goal of minimizing intra-cluster variance.

It is one of the most widely used clustering algorithms due to its simplicity, efficiency, and scalability.

---

## Learning Objectives

- Understand centroid-based clustering  
- Learn how K-Means forms clusters iteratively  
- Analyze the impact of K (number of clusters)  
- Evaluate clustering performance using standard techniques  

---

## Problem Formulation

Given a dataset X = {x₁, x₂, ..., xₙ}, the objective is to partition the data into K clusters:

C = {C₁, C₂, ..., Cₖ}

Such that the following objective is minimized:

Sum of Squared Distances (Inertia):

J = Σ Σ ||x - μⱼ||²

Where:
- μⱼ is the centroid of cluster Cⱼ  
- x represents data points assigned to cluster Cⱼ  

---

## Algorithm Workflow

1. Initialize K centroids (randomly or using K-Means++)  
2. Assign each data point to the nearest centroid  
3. Recompute centroids as the mean of assigned points  
4. Repeat steps 2 and 3 until convergence:
   - Centroids do not change significantly  
   - Maximum iterations reached  

---

## Key Concepts

### Centroid
The mean position of all data points in a cluster.

### Inertia (Within-Cluster Sum of Squares)
Measures how tightly data points are grouped within clusters.

### Convergence
Occurs when cluster assignments no longer change.

---

## Distance Metrics

K-Means relies on distance calculations, commonly:

- Euclidean Distance  
- Manhattan Distance (less common)  

Euclidean distance is typically used as it aligns with variance minimization.

---

## Choosing the Optimal K

### Elbow Method
Plots inertia against number of clusters (K). The optimal K is at the "elbow point" where the rate of decrease sharply changes.

### Silhouette Score
Measures how similar a point is to its own cluster compared to other clusters.

---

## Advantages

- Simple and easy to implement  
- Computationally efficient  
- Scales well to large datasets  
- Works well with spherical clusters  

---

## Limitations

- Requires predefined number of clusters (K)  
- Sensitive to initial centroid placement  
- Assumes clusters are spherical and equally sized  
- Struggles with outliers and noise  
- Poor performance on non-linear or complex cluster shapes  

---

## Improving Performance

- Use **K-Means++ initialization** for better centroid selection  
- Run algorithm multiple times and choose best result  
- Normalize or standardize features before clustering  
- Combine with PCA for dimensionality reduction  

---

## Applications

- Customer segmentation  
- Market analysis  
- Image compression  
- Document clustering  
- Recommendation systems  

---

## Evaluation Techniques

- Inertia (Within-cluster variance)  
- Silhouette Score  
- Visual inspection (2D/3D projections)  
- Comparison across multiple K values  

---

## Practical Considerations

- Feature scaling is essential for distance-based clustering  
- High dimensionality can affect performance  
- Sensitive to outliers — preprocessing is important  
- Initialization significantly impacts results  

---

## Implementation in This Repository

This module includes:

- K-Means implementation  
- Experiments with different K values  
- Visualization of cluster assignments  
- Evaluation using inertia and silhouette score  

---

## Repository Structure

K-Means/

├── implementation notebooks  
├── experiments  
└── README.md  

---

## Key Takeaways

- K-Means clusters data based on proximity to centroids  
- Efficient and scalable for large datasets  
- Requires careful selection of K  
- Works best for well-separated, spherical clusters  

---

## Conclusion

K-Means is a foundational clustering algorithm that provides an efficient way to partition data into meaningful groups. While simple in design, it is highly effective when applied to appropriately structured data and serves as a baseline for more advanced clustering techniques.
