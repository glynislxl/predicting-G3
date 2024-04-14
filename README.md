# predicting G3
Mini-Project for SC1015 - Introduction to Data Science and Artificial Intelligence
Lab: FCED
Group: 2

---

# About
This repository contains all the Jupyter Notebooks, dataset, video presentation and the source materials/references we have used and created as part of the Mini Project.

This README breifly highlights what we have accomplished in the project. If you want a more detailed explanation of things, please refer to the Jupyter Notebooks in this repository. They contain more in-depth descriptions and smaller details which are not mentioned here in the README. For convenience, we have divided the notenooks into smaller parts.

---

# Table of contents
1. [Problem definition](#problem-definition)
2. [Data preparation and Cleaning](#data-preparation-and-cleaning)
3. [Exploratory Data Analysis on Numeric Variables](#exploratory-data-analysis-on-numeric-variables)
4. [Exploratory Data Analysis on Categorical Variables](#exploratory-data-analysis-on-categorical-variables)
5. [Predictive modeling using Random Tree Forest](#predictive-modeling-using-random-tree-forest)
6. [Conclusion](#conclusion)
7. [References](#references)
8. [Learning Outcomes](#learning-outcomes)
   
---

# Problem Definition
Our Dataset: https://archive.ics.uci.edu/dataset/320/student+performance 

Our Question: Which predicators are the most accurate / reliable in  determining the future score (G3) ?

Success : determine future score (G3) using the predicators we found that are accurate / reliable

Rationale : By understanding which predictors have the strongest association with future scores, you can build more effective predictive models. This can lead to better allocation of resources and interventions to support students who may be at risk of achieving lower scores.

# Data Preparation and Cleaning
In this section of the project, we prepped and cleaned the dataset to help us to analyze our data better and also to help us use our data for the purposes of machine learning in the later sections.

We performed the following:
1. **Preliminary variable selection** : 8 relevant variables (3 numerical and 5 categorical) out of 33 were selected
2. **Encoding numeric variable**: the numeric variable were encoded appropriately by assigning letter grades to the respective numeric scores and adding a new column to the dataset
3. **Removing outliers for numeric variables**
4. **Converting Categorical Data to Numerical Data using One-Hot Encoding**, producing a separate data frame with a column per category 
Eg. 4 Categories (A-D) , if row n has value of A, under the column for A it has a value of 1, for columns B-D is has value of 0

# Exploratory Data Analysis on Numeric Variables
Then, we performed **linear regression** on 3 numeric variables (absences, health and studytime)

In our exploratory data analysis, the decision to utilize **K-fold cross-validation** was driven by several important considerations. 
1. Given the relatively small size of our dataset (~650 entries), the risk of overfitting while performing linear regression on our numeric variables (absences, health, and studytime) is significantly heightened.
- K-fold cross-validation addresses this issue effectively by dividing the entire dataset into 'K' number of subsets, thereby allowing the model to be trained and validated multiple times across different segments of data.
- This method enhances the reliability of the model by ensuring that every data point gets to be part of both the training and validation sets across the folds.
- Additionally, it improves the generalizability of our findings, making our regression model more robust against different samples of data.

By leveraging K-fold cross-validation, we can achieve a more accurate and consistent estimation of model performance, an essential factor in our analysis given the limited data size.

Based on the mean R^2 scores obtained from the analysis, it appears that the **'studytime' variable demonstrates the highest predictive accuracy among the numeric variables assessed**, with a mean R^2 score of approximately 0.0516. This indicates that 'studytime' has a relatively stronger association with the target variable ('G3' grades) compared to the other numeric variables. On the other hand, 'absences' yielded a mean R^2 score of around 0.0314, suggesting a somewhat lower predictive power compared to 'studytime'. Lastly, 'health' exhibited the lowest mean R^2 score of approximately 0.00308, indicating the weakest predictive capability among the numeric variables examined. 

Therefore, based on these results, we concluded that 'studytime' is the most accurate numeric predictor of 'G3' grades within the given dataset.
# Exploratory Data Analysis on Categorical Variables
Next, we used **decision tree model** on 5 categorical variables (address, paid, activities, higher education and reason)


# Predictive modeling using Random Tree Forest

# Conclusion


# References
- https://archive.ics.uci.edu/dataset/320/student+performance
- https://medium.com/@bididudy/the-essential-guide-to-k-fold-cross-validation-in-machine-learning-2bcb58c50578

# Learning Outcomes

---

# Contributors
- @glynislxl - Data Cleaning , Predictive modeling
- Wang Xin Ping - Exploratory Data Analysis on numeric variables
- Goh Qing Wen - Exploratory Data Analysis on categorical variables
