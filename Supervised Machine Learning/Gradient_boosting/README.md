# Gradient Boosting

---

## Files Included

| File | Description |
|:---|:---|
| `Gradient_boosting.ipynb` | Jupyter notebook with full implementation of Gradient Boosting |
| `student_depression_dataset.csv` |[Source: Kaggle Dataset - Student Depression](https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset/data)|

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
2. Gradient_boosting.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## Introduction

**Gradient Boosting** is a powerful ensemble learning technique based on boosting. It is widely used for both classification and regression tasks in supervised learning. Gradient Boosting works by combining multiple weak learners in a stage-wise fashion to form a strong learner.

![Gradient](./Gradient_boosting.jpg)

---

## Core Idea

Assume the target function \( F(x) \) can be represented as a sum of simple base learners \( f_k(x) \):

![Gradient](./Gradient_boosting1.jpg)

Each learner is trained sequentially to **minimize the loss** with respect to the current residuals (errors from the previous stage).

---

## Loss Function Minimization

At each step \( m \), the model fits a new learner \( f_m(x) \) to the negative gradient of the loss function, gradually reducing prediction errors.

### Common loss functions:

- **Mean Squared Error (MSE)** — for regression tasks
![Gradient](./Gradient_boosting2.jpg)

- **Log Loss** — for binary classification
![Gradient](./Gradient_boosting3.jpg)

- **Huber Loss**
![Gradient](./Gradient_boosting5.jpg)

- **Least Absolute Deviations (L1 Loss))**
![Gradient](./Gradient_boosting4.jpg)

---

## Gradient Descent in Function Space

Instead of adjusting weights in parameter space, Gradient Boosting performs gradient descent **in function space** — updating models by minimizing the loss function iteratively.

---

## Model Structure

- **Base learners**: Most often decision trees (especially CART)
- **Additive model**: Each new tree corrects the errors of the sum of previous trees

---

## Hyperparameter Tuning

Key hyperparameters to tune:

- `n_estimators`: Number of boosting stages
- `max_depth`: Maximum depth of each tree
- `learning_rate`: Shrinkage factor to control contribution of each tree
- `alpha`: Regularization parameter (e.g., L1)

---

## Advantages

- **High accuracy**: Ensemble learning significantly boosts prediction performance
- **Handles missing data**
- **Strong modeling power for non-linear relationships**

---

## Common Applications
### Financial services:
- Credit risk scoring
- Default prediction
- Investment strategy modeling

### Insurance:
- Premium estimation
- Claim amount prediction
- Risk-based pricing

### Healthcare:
- Disease diagnosis
- Cost forecasting

### Advertising:
- Click-through rate (CTR) prediction
- Target group segmentation

### E-commerce:
- Product recommendation systems
- Sales forecasting

### Education:
- Dropout prediction
- Learning outcome prediction

---

## 🧾 Conclusion

Gradient Boosting is one of the most effective and widely used ensemble learning techniques in modern machine learning. With its powerful predictive capabilities and flexible model structure, it is an indispensable tool in real-world data science projects.

---

## Reference:
Rednote: 94116033432
