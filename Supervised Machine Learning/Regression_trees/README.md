# Regression Trees

---

## Files Included

| File | Description |
|:---|:---|
| `Regression_trees.ipynb` | Jupyter notebook with full implementation of Regression Trees |
| `mudah-apartment-kl-selangor.csv` | The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/ariewijaya/rent-pricing-kuala-lumpur-malaysi?resource=download), containing around 19000 rental listings scraped from mudah.my, one of Malaysia’s major property platforms |

---

## Dataset Overview
Dataset includes 13 features and 1 target variable:

**Target**: `monthly_rent` – monthly rental price in Malaysian Ringgit (RM)

**Key Features:**
- `ads_id:` the listing ids (unique)
- `prop_name`: name of the building/ property
- `completion_year`: completion/ established year of the property
- `location`: property location in Kuala Lumpur region
- `property_type`:property type such as apartment, condominium, flat, duplex, studio, etc
- `rooms:` number of rooms in the unit
- `parking`: number of parking space for the unit
- `bathroom`: number of bathrooms in the unit
- `size`: total area of the unit in square feet
- `furnished`: furnishing status of the unit (fully, partial, non-furnished)
- `facilities:` main facilities available
- `additional_facilities:` additional facilities (proximity to attraction area, mall, school, shopping, railways, etc)

---

## How to Run
1. Clone the repository.
2. Regression_trees.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## Introduction

A **Regression Tree** is a type of decision tree used to predict continuous numerical outcomes by recursively splitting the data into smaller groups based on input features.

![What is a Regression Tree](regression2.png)


---

## How Regression Trees Work

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

## Simple Example

Below is a simple regression tree example:

- First split: "Is Age < 30?"
- If No: then "Is Income > 50k?"

Each final leaf predicts an average target value.

![Simple Regression Tree Example](regression1.png)

---

## Files Included

| File | Description |
|:---|:---|
| `Regression_trees.ipynb` | Jupyter notebook with full implementation of linear regression |
| `mudah-apartment-kl-selangor.csv` | Dataset used for model training and testing |

---

## How to Run

1. Clone the repository.
2. Open `Regression_trees.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

# Summary

Regression Trees are easy to interpret, capable of modeling complex non-linear relationships, and form the basis for more powerful ensemble models like Random Forests and Gradient Boosting.

---

## Reference
- rednote: 452924284
