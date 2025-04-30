# 🔍 Logistic Regression

## 📚 Core Concepts

**Logistic Regression** is a widely used classification method in statistics and machine learning, especially for **binary classification** tasks.  
Despite its name including the word "regression", it is fundamentally a **classification** algorithm.

Unlike linear regression, which can produce outputs outside of the [0, 1] range, logistic regression uses the **logistic (sigmoid)** function to **bound predicted values between 0 and 1**, representing the **probability** of an event occurring.

![Logistic vs Linear Regression](./34541746045632_.pic_resized.jpg)

---

## 🧠 How Logistic Regression Works

Logistic regression estimates the **probability** of a binary outcome based on input features.  
The logistic function is defined as:

\[
P(Y = 1 \mid X) = \frac{1}{1 + e^{-(\beta_0 + \beta_1 X_1 + \beta_2 X_2 + \cdots + \beta_p X_p)}}
\]

Taking the log-odds:

\[
\log\left(\frac{p}{1 - p}\right) = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \cdots + \beta_p X_p
\]

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
