# Neural Network

---

## Files Included

| File | Description |
|:---|:---|
| `Neural_networks.ipynb` | Jupyter notebook with full implementation of Neural Networks |
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
2. Neural_networks.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## Introduction

![A Simple Neural Network](./Neural_networks.jpg)

The diagram above illustrates a basic **feedforward neural network**. It consists of:
- **Input Layer**: Receives raw features (e.g., age, CGPA, sleep hours, etc.).
- **Hidden Layer**: Transforms input signals using learned weights and nonlinear activations (e.g., sigmoid).
- **Output Layer**: Produces the final prediction (in this case, the probability of depression).

## Mathematical Formulation
For a single-hidden-layer neural network:

![A Simple Neural Network](./Neural_network.jpg)

## Why Neural Networks?
Can capture complex non-linear relationships.

Handles both numeric and categorical features well.

Works effectively with behavioral and survey-type data like this depression dataset.

## Reference:
https://www.investopedia.com/terms/n/neuralnetwork.asp
