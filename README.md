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
1. preliminary variable selection : 8 relevant variables (3 numerical and 5 categorical) out of 33 were selected
2. encoding numeric variable : the numeric variable were encoded appropriately by assigning letter grades to the respective numeric scores and adding a new column to the dataset
3. removing outliers for numerical variables
4. Converting Categorical Data to Numerical Data using One-Hot Encoding, producing a separate data frame with a column per category 
Eg. 4 Categories (A-D) , if row n has value of A, under the column for A it has a value of 1, for columns B-D is has value of 0

# Exploratory Data Analysis on Numeric Variables

# Exploratory Data Analysis on Categorical Variables

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
