# Supervised Learning

# 1. What is Supervised Learning?

Supervised learning is a key branch of machine learning where models are trained on labeled datasets. 
Each training example consists of an input (features) and a correct output (label). 
The model learns a mapping from inputs to outputs, allowing it to make predictions on new, unseen data.

It’s widely applied in domains like:
- Email spam classification  
- Image recognition  
- Credit scoring  
- Sales forecasting  

Supervised learning algorithms fall into two major categories:
- Classification – predicting discrete labels (e.g., spam or not spam)  
- Regression – predicting continuous values (e.g., housing price)


# 2. How It Works?

1. Input features and output labels are used to train the model.
2. A loss function measures the prediction error.
3. The model adjusts its internal parameters (e.g., weights) to minimize the loss.
4. Evaluation is done on validation/test sets to measure generalization.

# 3. Why Use Supervised Learning?

- Clear objectives and measurable accuracy  
- Wide range of mature algorithms  
- Applicable to both classification and regression problems  
- Used in real-world decision systems across industries

# 4. What Models Belong to Supervised Learning?
Supervised learning includes a wide variety of models used for either regression or classification tasks.

In my GitHub repository, I include the following supervised learning models::

## Regression Models

Used when the target variable is continuous.
- Linear Regression
- Regression Trees

## Classification Models

Used when the target variable is categorical.
- The Perceptron
- Logistic Regression
- Neural Networks
- K-Nearest Neighbors (KNN)
- Random Forests
- Gradient Boosting

# 5. Datasets Used in This Project

## A. Regression Dataset – Kuala Lumpur Rental Prices
In this project, I applied Linear Regression and Regression Trees to predict monthly rent prices for residential properties in Kuala Lumpur and Selangor, Malaysia.
- Target Variable: monthly_rent (in Malaysian Ringgit)
- Size: ~19,000 rows
- Key Features: completion_year, location, property_type, rooms, parking, size, furnished, and more
The goal was to build a regression model that can estimate rent prices based on property characteristics.
For detailed dataset desceiption including dataset link, please refer to the python project file.

## B. Classification Dataset – Student Depression

I also worked on a binary classification task using the Student Depression Dataset, aimed at identifying mental health risks.

Target Variable: Depression
1 = student shows signs of depression
0 = student does not

Size: 27,901 students × 18 features

Key Features:
Demographics: Gender, Age, City
Academics: CGPA, Academic Pressure, Study Satisfaction
Lifestyle: Sleep Duration, Dietary Habits, Work Pressure, Work/Study Hours
Other: Financial Stress, Suicidal Thoughts, Family Mental Health History

This dataset was used to train classification models we listed above to predict whether a student is at risk of depression based on academic, lifestyle, and demographic indicators.

For detailed dataset desceiption including dataset link, please refer to the python project file.
