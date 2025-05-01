# Random Forest: A Powerful Ensemble Learning Algorithm

---

## Files Included

| File | Description |
|:---|:---|
| `Random_forests.ipynb` | Jupyter notebook with full implementation of Random Forests |
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
2. Random_forests.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## What is Random Forest?

Random Forest is an ensemble learning algorithm that builds multiple decision trees and combines their outputs. Each tree gives a prediction, and the forest makes the final decision by majority vote (for classification) or averaging (for regression).

Think of it like consulting multiple experts—each may have their own perspective, and the final answer is based on a collective decision.

![Random Forest Structure](images/Random_forests8.jpg)

---

## Why Use Multiple Trees?

One tree can easily be biased or overfit. But when you train many trees on different subsets of the data and features, each brings unique insights. By combining their results, the overall prediction becomes more stable and accurate.

---

## How is the "Forest" Built?
1. **Bootstrap Sampling**: Each tree is trained on a random subset of the data (with replacement).
2. **Random Feature Selection**: At each split in a tree, a random subset of features is considered for splitting, not all of them.
3. **Tree Construction**: Repeat the above steps to grow many trees, then aggregate their predictions.

![Random Forest Workflow](images/Random_forests.jpg)

---

## Formula:  
![Random Forest Workflow](images/Random_forest.jpg)

---

## Where is the Randomness?

- **Random Data**: Each tree uses a different bootstrap sample.
- **Random Features**: Each split considers a random subset of features.

This randomness makes each tree slightly different, helping reduce overfitting and improve generalization.

---

## Why is Random Forest So Popular?

- High Accuracy: Ensemble of multiple trees usually outperforms a single decision tree.
- Easy to Use: It works well even with minimal hyperparameter tuning.
- Parallelizable: Trees are built independently, making it easy to train on large datasets.

---

## Summary

Random Forest combines the strengths of many decision trees to create a high-performance model.

---

## Reference
Rednote: 192052443

