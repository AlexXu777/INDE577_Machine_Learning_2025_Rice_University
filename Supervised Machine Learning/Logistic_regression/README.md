# 🔍 Logistic Regression

## 📚 Core Concepts

**Logistic Regression** is a widely used classification method in statistics and machine learning, especially for **binary classification** tasks.  
Despite its name including the word "regression", it is fundamentally a **classification** algorithm.

Unlike linear regression, which can produce outputs outside of the [0, 1] range, logistic regression uses the **logistic (sigmoid)** function to **bound predicted values between 0 and 1**, representing the **probability** of an event occurring.

---

## 🧠 How Logistic Regression Works

Logistic regression estimates the **probability** of a binary outcome based on input features.  
The logistic function is defined as:

![Logistic vs Linear Regression](./Logistic_regression1.jpg)

Taking the log-odds:

![Logistic vs Linear Regression](./Logistic_regression2.jpg)
- The model parameters are estimated using **Maximum Likelihood Estimation (MLE)**.
- The predicted probability is converted into class labels using a **threshold** (commonly 0.5).

![Formula and Explanation](./34551746045636_.pic_resized.jpg)

---

## ⚙️ Example in R

We use the `Default` dataset to predict whether a person will default on their credit based on income, balance, and student status.

```r
# Load libraries and data
library(ISLR)
data("Default")

# Fit logistic regression
logit.fit <- glm(default ~ income + balance + student, data = Default, family = binomial)

# View model summary
summary(logit.fit)
