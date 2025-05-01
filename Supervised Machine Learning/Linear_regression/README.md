# Linear Regression
A project demonstrating the key concepts, mathematical formulations, and implementation of linear regression models.

---

## Files Included

| File | Description |
|:---|:---|
| `Linear_regression.ipynb` | Jupyter notebook with full implementation of linear regression |
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

## How to Run

1. Clone the repository.
2. Open `Linear_regression.ipynb` in Jupyter Notebook.
3. Run all the cells step-by-step to reproduce the results.

---

## Core Concepts

### 1. Assume a Linear Relationship
There exists a linear relationship between the dependent variable \( y \) and the independent variable(s) \( x \).  
In other words, the output is a weighted linear combination of the input features.

![Linear Regression Illustration](linear1.png)

---

### 2. Minimize the Error
The model aims to minimize the difference between the predicted values and the actual values.  
This is typically achieved by minimizing the **Mean Squared Error (MSE)**.

![Mean Squared Error](mse1.png)

---

### 3. Strong Interpretability
Each regression coefficient reflects how much a particular input feature contributes to the output,  
including the direction of the relationship (positive/negative correlation).

---

## Mathematical Formulas

### Simple Linear Regression (with one independent variable)

\[
y = wx + b
\]

- \( x \): Independent variable (input feature)
- \( y \): Dependent variable (target/predicted value)
- \( w \): Regression coefficient (weight/slope)
- \( b \): Bias term (intercept)

---

### Multiple Linear Regression (with multiple independent variables)

![Multiple Linear Regression](Multiple%20Linear%20Regression.png)

The goal is to find the optimal parameters \( w \) and \( b \)  
to minimize the prediction error on the training data.

---

## 📎 Reference

- [Linear Regression - Wikipedia](https://en.wikipedia.org/wiki/Linear_regression)
- rednote: 5860288153
- Rice University - INDE577 Machine Learning Course Materials
