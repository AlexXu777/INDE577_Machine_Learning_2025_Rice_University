# 🧠 Artificial Neuron (Perceptron Model)

This repository illustrates how an **Artificial Neuron**, also known as a **Perceptron**, works from a mathematical and visual perspective. It is one of the foundational models for binary classification problems in machine learning.

---

## 🔬 What is an Artificial Neuron?

An **Artificial Neuron** is a fundamental component in machine learning models, especially neural networks. It receives multiple inputs, applies weights and bias, and produces a binary output using an activation function.

![Neuron Intro](./34651746047842_.pic.jpg)

---

## ⚙️ Key Components of the Neuron

### 1. Inputs and Weights

- \( x = (x_1, x_2, \dots, x_m) \): the input features  
- \( w = (w_1, w_2, \dots, w_m) \): the weights assigned to each input

The dot product of weights and inputs is computed as:

\[
z = w_1x_1 + w_2x_2 + \cdots + w_mx_m
\]

![Inputs and Weights](./34661746047843_.pic.jpg)

---

### 2. Decision Function

The output \( z \) is passed through a decision function, typically a **step function** (hard threshold):

\[
\sigma(z) =
\begin{cases}
1 & \text{if } z \geq \theta \\
0 & \text{if } z < \theta
\end{cases}
\]

![Decision Function](./34671746047844_.pic.jpg)

---

### 3. Simplification with Bias

To simplify the decision logic, we define a new parameter \( b = -\theta \), and the condition becomes:

\[
z = w_1x_1 + w_2x_2 + \cdots + w_mx_m + b
\]

This is the final expression of the perceptron's linear combination with a bias term.

![Simplification](./34681746047845_.pic.jpg)

---

## ✅ Final Representation

The final mathematical formulation of an artificial neuron is:

\[
z = \sum_{i=1}^{n} w_i x_i + b
\quad
\sigma(z) =
\begin{cases}
1 & \text{if } z \geq 0 \\
0 & \text{if } z < 0
\end{cases}
\]

This function classifies inputs into two categories depending on whether the weighted sum exceeds a threshold.

![Final Representation](./34701746047847_.pic.jpg)

---

## 🔁 Functional View

Here’s a complete view of how inputs, weights, bias, and activation come together:

1. Inputs are combined through a **weighted summation**
2. A **bias** is added
3. The result is passed through an **activation function**

![Functional Diagram](./34711746047848_.pic.jpg)

---

## 🧩 Summary

- The **Perceptron** is a simple yet powerful model for binary classification.
- It mimics a biological neuron with inputs, weights, and activation.
- This model serves as the **foundation for more complex neural networks**, such as multi-layer perceptrons (MLPs) and deep learning architectures.

---

## 📦 Files Included

| File | Description |
|------|-------------|
| `perceptron.py` | Python implementation of the Perceptron model |
| `README.md` | This file |
| `images/` | All neuron-related images used in this markdown |

---

## 📚 Reference

- [Towards Data Science - Neural Networks](https://towardsdatascience.com)
- Credit for all visuals: **Píldoras de Programación**
你可以将以上内容保存为 README.md 文件，配套存放相关图片（文件名保持不变或统一放入 images/ 文件夹，并调整路径）。

需要我打包 .md 文件并帮你改图路径或生成 .zip 吗？







您说：
不要任何Artificial Neuron ，只保留Perceptron Model


ChatGPT 说：
好的！以下是专注于 Perceptron Model 的 README.md 文件内容，已去除所有 "Artificial Neuron" 表述，专注于感知机（Perceptron）的原理、组成、公式和可视图解说明，并用 .md 格式组织好，适合配套图片一起使用：

markdown
复制
编辑
# 🧠 Perceptron Model

This repository introduces the **Perceptron Model**, a fundamental algorithm for binary classification tasks in machine learning. It is the building block for more complex models such as neural networks.

---

## 📌 Overview

The Perceptron receives multiple inputs, applies weights and bias, and produces a binary output using a threshold-based activation function.

---

## ⚙️ Key Components

### 1. Inputs and Weights

Each input feature \( x_i \) is multiplied by a corresponding weight \( w_i \). The weighted sum is calculated as:

\[
z = w_1x_1 + w_2x_2 + \cdots + w_mx_m
\]

This operation determines how much influence each input has on the output.

![Inputs and Weights](./34661746047843_.pic.jpg)

---

### 2. Decision Function

After calculating the weighted sum \( z \), the model applies a step function to decide the output class:

\[
\sigma(z) =
\begin{cases}
1 & \text{if } z \geq \theta \\
0 & \text{if } z < \theta
\end{cases}
\]

Where \( \theta \) is a manually defined threshold.

![Decision Function](./34671746047844_.pic.jpg)

---

### 3. Simplification with Bias

To simplify the model, we define a bias term \( b = -\theta \), and the formula becomes:

\[
z = w_1x_1 + w_2x_2 + \cdots + w_mx_m + b
\]

This helps make the threshold part of the learned parameters during training.

![Simplification](./34681746047845_.pic.jpg)

---

## ✅ Final Representation

Putting it all together, the final Perceptron model is represented as:

\[
z = \sum_{i=1}^{n} w_i x_i + b
\quad
\sigma(z) =
\begin{cases}
1 & \text{if } z \geq 0 \\
0 & \text{if } z < 0
\end{cases}
\]

This function outputs 1 or 0 based on whether the input passes the learned decision boundary.

![Final Representation](./34701746047847_.pic.jpg)

---

## 🔁 Functional Architecture

The Perceptron structure includes:

1. A **weighted summation** of inputs
2. Addition of a **bias**
3. Application of an **activation function** (step function)

![Perceptron Diagram](./34711746047848_.pic.jpg)

---
