# Principal Component Analysis (PCA)

## What is PCA?

Principal Component Analysis (PCA) is one of the most widely used **dimensionality reduction** techniques. It transforms high-dimensional data into a lower-dimensional feature space while preserving as much **variance** as possible.

PCA identifies new axes, called **principal components**, that are linear combinations of the original variables. These components are uncorrelated and ordered by the amount of variance they capture.

![K_means_clustering](./PCA1.jpg)

---

## 📐 Mathematical Formulation

Given a zero-centered dataset \( X \in \mathbb{R}^{n \times d} \):

1. **Compute the covariance matrix**:
   \[
   \mathbf{S} = \frac{1}{n} X^\top X
   \]

2. **Compute eigenvalues and eigenvectors**:
   \[
   \mathbf{S} \mathbf{u}_i = \lambda_i \mathbf{u}_i
   \]

3. **Sort eigenvectors** by descending eigenvalues:
   \[
   \lambda_1 \geq \lambda_2 \geq \dots \geq \lambda_d
   \]

4. **Project data to new subspace**:
   \[
   Z = X \mathbf{U}_k
   \]

📷 _[Insert Image: “什么是主成分分析”]_  
📷 _[Insert Image: “PCA 工作步骤 (公式版)”]_

---

## 🔧 PCA Workflow

1. **Standardize the data**: ensure zero mean and unit variance.
2. **Compute the covariance matrix** to capture relationships between features.
3. **Eigen decomposition** to extract principal components.
4. **Select top K components** with the highest eigenvalues.
5. **Transform original data** to the new subspace.

📷 _[Insert Image: “PCA 工作步骤 (中文文字版)”]_

---

## ✅ Why Use PCA?

- **Noise Reduction**: Filter out noise to highlight key structure.
- **Visualization**: Project high-dimensional data into 2D/3D space.
- **Efficiency**: Reduce model complexity and training time.
- **Improve Performance**: Remove irrelevant or redundant features.

📷 _[Insert Image: “PCA 用途”]_

---

## 📊 Real-World Applications

- 🖼️ **Image Processing**: Feature extraction, denoising, compression.
- 💹 **Finance**: Portfolio optimization, risk modeling.
- 🧬 **Bioinformatics**: Disease gene prediction, genome analysis.

---

## 🧪 PCA in This Project

In this project, PCA is applied to the Fashion MNIST dataset to reduce the original **784-dimensional pixel space** to a lower-dimensional subspace before applying clustering or visualization. This improves interpretability and reduces computational cost.

> 📌 *Note: PCA was implemented manually and applied as part of the unsupervised learning model comparison.*


