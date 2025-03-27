Titanic Competition - Kaggle Challenge

The goal is to predict if a passenger will survive based on features like age, sex, and more.

## Project objectives

- Clean and preprocess the dataset using `pandas`
- Convert categorical variables into numerical format
- Train a machine learning model to classify survival
- Generate predictions and submit results to Kaggle

## Model used

# Logistic Regression

I used a logistic regression for mainly two reasons:

First, I'm still a beginner in those domaines (machine learning and data science) and Logistic Regression is easy to understand. Then, the logistic regression is well-suited for binary classification problems like this one.


## Methodology

#1. Data Cleaning
- Replaced missing values in `Age` with the median
- Dropped the `Cabin` column due to too many missing values
- Replaced missing values in `Embarked` with the most frequent category

#2. Feature Engineering
   - Encoded `Sex` (0 = male, 1 = female)
   - One-hot encoded `Embarked`
   - Dropped unnecessary columns: `Ticket`, `Name`, `Cabin`

#3. Modeling
   - Split the data into 80% training and 20% validation sets
   - Trained a Logistic Regression model using `scikit-learn`
   - Generated predictions on the test set


##Results

Kaggle public score: 77,5 %



## Files in this repository

Titanic_notebook.ipynb -> Main notebook, contains the python code.
requirements.txt -> List of required libraries
data/ -> contains the datasets that Kaggle gives us to realise this project
