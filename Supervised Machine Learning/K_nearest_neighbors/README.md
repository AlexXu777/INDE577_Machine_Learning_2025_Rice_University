# K-Nearest Neighbors (KNN)

---

## Files Included

| File | Description |
|:---|:---|
| `K_nearest_neighbors.ipynb` | Jupyter notebook with full implementation of K Nearest Neighbors |
| `student_depression_dataset.csv` | [Source: Kaggle Dataset - Student Depression](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset/data)|

---

## Dataset Overview
The Student Depression Dataset is designed to analyze mental health trends and key predictors among students. It combines demographic, academic, and lifestyle information to identify factors associated with depression.

**Data Format:**
*  CSV file, one row per student
*  Total rows: 27,901
*  Total columns: 18

**Variable Categories:**
*   Demographics: Gender, Age, City
*   Academic Factors: CGPA, Academic Pressure, Study Satisfaction
*   Lifestyle: Sleep Duration, Dietary Habits, Work Pressure, Work/Study Hours
*   Additional: Degree, Profession, Financial Stress, Family History of Mental Illness, and suicidal thoughts

**Target Variable**: `Depression`  
*   `1` indicates the student is experiencing symptoms of depression
*   `0` indicates the student is not experiencing depression

---

## How to Run
1. Clone the repository.
2. K_nearest_neighbors.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## Introduction
K-Nearest Neighbors (KNN) is a **simple yet powerful** non-parametric classification algorithm. It predicts the class of a sample based on the majority class among its **k closest neighbors** in the feature space.

![KNN](./K_nearest_neighbors1.jpg)

## Core Idea

The KNN algorithm is based on a **distance metric**. To classify a new point:

1. Calculate the distance from the point to be predicted to all points in the training set.
2. Select the **k nearest neighbors** (smallest distances).
3. Perform a **majority vote** to decide the class label.

### Euclidean Distance Formula

The most common distance metric used is **Euclidean distance**:

![KNN](./K_nearest_neighbors.jpg)

Where:
- x is the test sample
- 𝑥i is a sample from the training dataset
- xj is the j-th feature of the test sample
- xij is the j-th feature of the training sample
- n is the number of features

---

## Advantages of KNN

- **Simple to understand**: No training phase; easy to implement
- **Non-parametric**: Makes no assumptions about data distribution
- **Naturally handles multi-class problems**
- **Flexible**: Works with any distance metric (e.g., Euclidean, Manhattan)
- **Effective in small, clean datasets** with well-separated classes

---

## Summary

K-Nearest Neighbors (KNN) is a straightforward but effective classification method. It uses the principle of “proximity voting” in feature space, making predictions based on the closest samples from the training set. While it lacks a training phase, its prediction time can be slow, especially for large datasets. However, with proper preprocessing (e.g., feature scaling) and a well-chosen \( k \), KNN remains a strong baseline for classification tasks.

---

## Reference:
Rednote: 94116033432
