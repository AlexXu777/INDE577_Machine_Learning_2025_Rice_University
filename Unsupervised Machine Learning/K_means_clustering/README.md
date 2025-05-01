# K-Means Clustering Model

This project implements the classic **K-Means Clustering** algorithm from scratch using Python and applies it to a large-scale dataset. The goal is to group unlabeled data into K distinct clusters based on feature similarity.

> Due to the large size of the full dataset, **this repository only includes the test set**. For the complete dataset, please refer to the link provided inside the Python code file.

---

## What is Clustering?
Clustering is a type of **unsupervised learning** algorithm that groups similar data points into clusters without needing labeled data.

Applications include:
- User segmentation (e.g., personalized ads, news grouping)
- Image segmentation & compression
- Data reduction and anomaly detection

![K_means_clustering](./K_means_clustering4.jpg)

---

## What is K-Means?
K-Means is a basic but powerful clustering algorithm. It aims to partition `n` observations into `K` clusters where each observation belongs to the cluster with the nearest mean (centroid).

![K_means_clustering](./K_means_clustering1.jpg)

---

## Mathematical Objective:

Minimize the **within-cluster sum of squared distances (WCSS)**:

![K_means_clustering](./K_means_clustering2.jpg)


![K_means_clustering](./K_means_clustering3.jpg)


---

## K-Means Algorithm Steps

![K_means_clustering](./K_means_clustering5.jpg)

1. **Initialization**: Randomly select K data points as initial centroids.
2. **Cluster Assignment**: Assign each point to the nearest centroid based on Euclidean distance.
3. **Update Step**: Recalculate centroids as the mean of the points in each cluster.
4. **Repeat**: Steps 2–3 until convergence (no change in centroids or cluster assignments).

---

## Choosing the Value of K

![K_means_clustering](./K_means_clustering8.jpg)

### Common Methods:
**Elbow Method**: Choose K at the “elbow” point where WCSS no longer decreases significantly.

---

## Advantages

- **Simple** and intuitive.
- **Fast** for datasets with a relatively small number of features.
- **Scalable** to large datasets with efficient implementations.

---
