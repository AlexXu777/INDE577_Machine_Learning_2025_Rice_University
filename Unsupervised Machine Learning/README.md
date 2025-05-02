# Unsupervised Learning

# 1. What is Unsupervised Learning?

Unsupervised learning is a type of machine learning where the model is trained on **unlabeled data**.  
Unlike supervised learning, the algorithm tries to find **hidden patterns or structures** in the input data without any ground truth labels.

It’s commonly used for:
- Customer segmentation  
- Anomaly detection  
- Dimensionality reduction  
- Market basket analysis  
- Image compression  

Key unsupervised learning categories include:
- **Clustering** – grouping similar data points together  
- **Dimensionality Reduction** – compressing data while retaining key patterns  

# 2. How It Works?

1. The model receives raw input data without labels.  
2. It tries to learn structure, similarity, or statistical patterns.  
3. It often uses distance metrics (e.g., Euclidean distance) or matrix factorization.  
4. The outcome may be clusters, compressed representations, or components.

# 3. Why Use Unsupervised Learning?

- No need for labeled data  
- Useful for data exploration and feature engineering  
- Often reveals insights humans might miss  
- Used in many real-world applications like recommendation systems and fraud detection

# 4. What Models Belong to Unsupervised Learning?

In this project, I implemented and tested the following unsupervised learning models:

- **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**  
- **K-Means Clustering**  
- **Principal Component Analysis (PCA)**  
- **Singular Value Decomposition (SVD)**

# 5. Datasets Used in This Project

## Fashion MNIST
The **Fashion MNIST** dataset, developed by Zalando Research, contains 70,000 grayscale images of fashion items—60,000 for training and 10,000 for testing. Each image is 28×28 pixels (flattened to 784 features). While labeled with one of 10 fashion categories, these labels were used only for evaluation in our unsupervised learning tasks.

**Key Specs:**
- **Total examples:** 70,000  
- **Image size:** 28 × 28 (grayscale)  
- **Classes:**  
  0 – T-shirt/top  
  1 – Trouser  
  2 – Pullover  
  3 – Dress  
  4 – Coat  
  5 – Sandal  
  6 – Shirt  
  7 – Sneaker  
  8 – Bag  
  9 – Ankle boot  

The goal was to uncover latent structure in urban mobility without using any labels.

For detailed dataset descriptions and preprocessing steps, please refer to the corresponding Python notebooks.
