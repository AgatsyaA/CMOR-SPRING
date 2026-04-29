# K-Nearest Neighbors (KNN)

<p align="center">
  <img src="https://miro.medium.com/0*ItVKiyx2F3ZU8zV5" width="600"/>
</p>

---

## Overview

**K-Nearest Neighbors (KNN)** is a supervised machine learning algorithm used for **classification** and **regression**. It makes predictions based on the **similarity (distance)** between data points.

KNN is a **non-parametric, instance-based (lazy learning)** algorithm that does not learn a model during training but instead stores the dataset and makes decisions at prediction time. :contentReference[oaicite:0]{index=0}

---

## How It Works

- Choose the number of neighbors \( k \)  
- Compute distance between the new data point and all training points  
- Select the **k closest neighbors**  
- Predict:
  - **Classification** → Majority vote  
  - **Regression** → Average of neighbors  

KNN assumes that **similar data points exist close to each other in feature space**. :contentReference[oaicite:1]{index=1}  

---

## Key Concepts

- **K Value** → Number of neighbors considered  
- **Distance Metric** → Measures similarity (e.g., Euclidean distance)  
- **Lazy Learning** → No explicit training phase  
- **Feature Scaling** → Important for accurate distance calculation  

---

## Distance Metrics

Common distance measures used in KNN:

- **Euclidean Distance**  
- **Manhattan Distance**  
- **Minkowski Distance**  

Distance plays a critical role since predictions depend on nearest neighbors. :contentReference[oaicite:2]{index=2}  

---

## Types of KNN

- **Classification KNN** → Predicts categorical labels  
- **Regression KNN** → Predicts continuous values  

---

## Choosing the Right K

- Small \( k \) → High variance, sensitive to noise  
- Large \( k \) → Low variance, may underfit  
- Optimal \( k \) is typically chosen using **cross-validation** :contentReference[oaicite:3]{index=3}  

---

## Advantages

- Simple and intuitive  
- No training time required  
- Works well with multi-class data  
- Flexible and easy to update  

---

## Limitations

- Computationally expensive for large datasets  
- Sensitive to irrelevant features  
- Performance degrades with high dimensions (curse of dimensionality)  
- Requires feature scaling  

---

## Applications

- Recommendation systems  
- Pattern recognition  
- Image classification  
- Medical diagnosis  

---
