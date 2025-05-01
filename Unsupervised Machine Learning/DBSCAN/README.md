# DBSCAN Clustering Algorithm

This repository implements the **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)** algorithm in Python. DBSCAN is a powerful density-based clustering method especially effective in identifying arbitrarily shaped clusters and dealing with noisy data.

---

## What is DBSCAN?

DBSCAN groups together points that are closely packed together (points with many nearby neighbors), marking as outliers the points that lie alone in low-density regions.

![K_means_clustering](./DBSCAN1.jpg)


By *Martin Ester et al. (1996)*, DBSCAN assumes that clusters are areas of **high density separated by low density**. Unlike K-Means, **DBSCAN does not require the number of clusters (K) to be specified** in advance and is robust to outliers.

---

## Key Concepts & Parameters

DBSCAN requires two parameters:
- **ε (epsilon)**: The radius of the neighborhood around a data point.
- **minPts**: The minimum number of points required to form a dense region (core point).

In high-dimensional data, this ε becomes a **hypersphere**.

---

## 🧠 Core Ideas

Each point is classified as one of the following:

- **Core Point**: Has at least `minPts` points within its ε-neighborhood.
- **Border Point**: Has fewer than `minPts` points in ε-neighborhood but is reachable from a core point.
- **Noise Point**: Not reachable from any core point.

![K_means_clustering](./DBSCAN2.jpg)

---

## 🧪 How It Works

For each point in the dataset:

1. Count how many points are within ε.
2. If at least `minPts`, label it a **core point**.
3. All points within its ε are **directly density-reachable**.
4. Cluster grows through **density-connected** points.

### 📐 Distance Metric

DBSCAN typically uses **Euclidean distance**:

![K_means_clustering](./DBSCAN3.jpg)

---

## 📊 Reachability & Connectivity

DBSCAN relies on two key notions:
- **Reachability**: Can a point be reached from another under ε and minPts?
- **Connectivity**: Can two points be linked through a sequence of density-reachable steps?

**Conditions for Direct Density Reachability:**
Point x is directly density-reachable from y if:
- dist(x,y)≤ϵ
- 𝑦 is a core point

![K_means_clustering](./DBSCAN4.jpg)

For **Density Reachability**:
If a chain \( p_1, p_2, ..., p_n \) exists where each \( p_{i+1} \) is directly density-reachable from \( p_i \), then \( p_n \) is density-reachable from \( p_1 \).

![K_means_clustering](./DBSCAN5.jpg)

---

## 🤔 Why Use DBSCAN?

K-Means and Hierarchical Clustering struggle with:
- Non-spherical clusters
- Varying densities
- Noisy data

DBSCAN handles all of the above effectively, making it suitable for tasks like:
- Anomaly detection
- Spatial data mining
- Arbitrary-shape pattern recognition

<p align="center">
  <img src="images/dbscan_ring_example.jpg" width="500"><br>
  <em>DBSCAN successfully identifies concentric clusters with varying density</em>
</p>

---

## 📁 Folder Structure

