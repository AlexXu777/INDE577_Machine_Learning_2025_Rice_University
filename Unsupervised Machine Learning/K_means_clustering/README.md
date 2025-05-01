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

![K_means_clustering](./K_means_clustering1.jpg)

---

## What is K-Means?
K-Means is a basic but powerful clustering algorithm. It aims to partition `n` observations into `K` clusters where each observation belongs to the cluster with the nearest mean (centroid).

### 🧮 Mathematical Objective:

Minimize the **within-cluster sum of squared distances (WCSS)**:

![K_means_clustering](./K_means_clustering2.jpg)


![K_means_clustering](./K_means_clustering3.jpg)


---

## 🛠️ K-Means Algorithm Steps

<p align="center">
  <img src="35701746075922_.pic.jpg" width="600">
</p>

1. **Initialization**: Randomly select K data points as initial centroids.
2. **Cluster Assignment**: Assign each point to the nearest centroid based on Euclidean distance.
3. **Update Step**: Recalculate centroids as the mean of the points in each cluster.
4. **Repeat**: Steps 2–3 until convergence (no change in centroids or cluster assignments).

---

## 🔢 Choosing the Value of K

<p align="center">
  <img src="35711746075924_.pic.jpg" width="400">
</p>

### Common Methods:
1. **Elbow Method**: Choose K at the “elbow” point where WCSS no longer decreases significantly.
2. **Silhouette Analysis**: Measures how similar a point is to its own cluster vs. other clusters (range -1 to 1).
3. **Domain Knowledge**: Use subject matter understanding to select K.

---

## ✅ Advantages

- **Simple** and intuitive.
- **Fast** for datasets with a relatively small number of features.
- **Scalable** to large datasets with efficient implementations.

<p align="center">
  <img src="35691746075921_.pic.jpg" width="500">
</p>

---

## ⚠️ Limitations

<p align="center">
  <img src="35721746075925_.pic.jpg" width="500">
</p>

- Requires predefining `K`, which may not be obvious.
- Sensitive to **initial centroids**.
- May converge to **local minima**.
- Assumes **spherical clusters** of similar size — not always realistic.

---

## 📁 Dataset

This model was tested using a real-world dataset (see `.py` file for link). The dataset contains unlabeled data points that were clustered into meaningful groups using K-Means. Due to GitHub storage limits, only a **test subset** is included in this repo.

---

## 📎 Folder Structure

