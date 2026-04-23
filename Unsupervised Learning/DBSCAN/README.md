# DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

<p align="center">
  <img src="https://ik.imagekit.io/upgrad1/abroad-images/imageCompo/images/img_0_1_86GN1D.png" width="600"/>
</p>

## Overview

DBSCAN is a density-based unsupervised learning algorithm used to cluster data points based on the concept of density connectivity. It groups points that are closely packed together while identifying points in low-density regions as noise.

Unlike centroid-based algorithms such as K-Means, DBSCAN does not require the number of clusters to be specified in advance and can identify clusters of arbitrary shape.

---

## Learning Objectives

- Understand density-based clustering principles  
- Learn how DBSCAN identifies clusters and outliers  
- Analyze the impact of ε (epsilon) and MinPts  
- Evaluate clustering performance and limitations  

---

## Key Concepts

### Core Points
A point is a core point if it has at least **MinPts neighbors within radius ε**.

### Border Points
Points that lie within the ε-neighborhood of a core point but do not satisfy the MinPts requirement themselves.

### Noise Points (Outliers)
Points that are neither core nor border points and do not belong to any cluster.

### Density Reachability
A point is directly reachable from another point if it lies within ε distance and the source point is a core point.

### Density Connectivity
Two points are density-connected if there exists a chain of points linking them through core points.

---

## Parameters

### Epsilon (ε)
Defines the radius used to determine the neighborhood of a point.

### MinPts
Minimum number of points required to form a dense region.

Choosing appropriate values for these parameters is critical for model performance.

---

## Algorithm Workflow

1. Select an unvisited point  
2. Retrieve all neighboring points within ε radius  
3. If neighbors ≥ MinPts:
   - Mark the point as a core point  
   - Create a new cluster  
   - Expand the cluster recursively using density reachability  
4. If neighbors < MinPts:
   - Mark as noise (can later become a border point)  
5. Repeat until all points are processed  

---

## Distance Metrics

DBSCAN relies on distance calculations. Common choices include:

- Euclidean Distance  
- Manhattan Distance  
- Cosine Distance  

The choice of distance metric affects cluster formation.

---

## Advantages

- Does not require specifying the number of clusters  
- Identifies clusters of arbitrary shape  
- Robust to noise and outliers  
- Works well for spatial and density-based data  

---

## Limitations

- Sensitive to ε and MinPts selection  
- Struggles with clusters of varying densities  
- Performance decreases in high-dimensional data  
- Distance metric choice impacts results  

---

## Parameter Selection Strategy

- Use **k-distance graph** to estimate ε  
- Set MinPts based on dimensionality (typically ≥ dimensions + 1)  
- Normalize or scale features before clustering  

---

## Applications

- Anomaly detection  
- Geospatial clustering  
- Customer segmentation  
- Image processing  
- Fraud detection  

---

## Evaluation Techniques

Since labels are unavailable, evaluation is indirect:

- Silhouette Score  
- Visual inspection of clusters  
- Cluster density analysis  
- Domain-specific validation  

---

## Practical Considerations

- Feature scaling is essential for distance-based clustering  
- High dimensionality can reduce effectiveness (curse of dimensionality)  
- Combining with PCA improves clustering quality  
- Noise handling is a key advantage over centroid-based methods  

---

## Implementation in This Repository

This module includes:

- DBSCAN implementation  
- Experiments with different ε and MinPts values  
- Visualization of clusters and noise points  
- Comparison with other clustering methods  

---

## Repository Structure

DBSCAN/

├── implementation notebooks  
├── experiments  
└── README.md  

---

## Key Takeaways

- DBSCAN clusters data based on density rather than distance to centroids  
- Automatically detects outliers  
- Effective for irregular cluster shapes  
- Requires careful parameter tuning for optimal results  

---

## Conclusion

DBSCAN is a powerful clustering algorithm for identifying meaningful structures in data without requiring prior knowledge of cluster count. Its ability to handle noise and detect arbitrarily shaped clusters makes it particularly useful for real-world datasets, especially in spatial and anomaly detection contexts.
