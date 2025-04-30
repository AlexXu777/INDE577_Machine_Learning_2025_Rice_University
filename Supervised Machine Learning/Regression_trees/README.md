# NOTE: If images fail to load, please refer to `README.ipynb` for a complete version with embedded visuals.

# 🌲 Regression Trees

---

## 📊 Files Included

| File | Description |
|:---|:---|
| `Regression_trees.ipynb` | Jupyter notebook with full implementation of Regression Trees |
| `mudah-apartment-kl-selangor.csv` | Dataset used for model training and testing |

---

## 🛠️ How to Run
1. Clone the repository.
2. Regression_trees.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## 📚 Core Concepts

A **Regression Tree** is a type of decision tree used to predict continuous numerical outcomes by recursively splitting the data into smaller groups based on input features.

![What is a Regression Tree](regression2.png)


---

## 🧠 How Regression Trees Work

Regression Trees work by:

- **Start with All Data**: Begin with the whole dataset at the root.
- **Find the Best Split**: Choose a feature and a split point that minimizes the prediction error (e.g., MSE).
- **Repeat for Each Branch**: Keep splitting until a stopping rule is met (such as minimum number of samples or maximum depth).
- **Make Predictions**: Predict by averaging the values in the final (leaf) nodes.

Common use cases include:

- House price prediction
- Predicting loan amounts
- Forecasting sales
- Estimating health outcomes

![How a Regression Tree Works](regression3.png)


---

## 🌳 Simple Example

Below is a simple regression tree example:

- First split: "Is Age < 30?"
- If No: then "Is Income > 50k?"

Each final leaf predicts an average target value.

![Simple Regression Tree Example](regression1.png)

---

## 📊 Files Included

| File | Description |
|:---|:---|
| `Regression_trees.ipynb` | Jupyter notebook with full implementation of linear regression |
| `mudah-apartment-kl-selangor.csv` | Dataset used for model training and testing |

---

## 🛠️ How to Run

1. Clone the repository.
2. Open `Regression_trees.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

# Summary

Regression Trees are easy to interpret, capable of modeling complex non-linear relationships, and form the basis for more powerful ensemble models like Random Forests and Gradient Boosting.

---

## Reference
- rednote: 452924284
