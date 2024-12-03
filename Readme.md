# Titanic Survival Prediction

This project aims to predict the survival of passengers aboard the Titanic based on various features using machine learning techniques.

## Overview

The Titanic dataset contains information about passengers, such as age, sex, class, ticket information, and other features that may affect survival rates. The goal of this project is to build a machine learning model that can predict whether a passenger survived or not.

## Dataset
- `PassengerId`: Unique ID for each passenger
- `Survived`: Whether the passenger survived (1) or not (0)
- `Pclass`: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: Name of the passenger
- `Sex`: Gender of the passenger (male/female)
- `Age`: Age of the passenger
- `SibSp`: Number of siblings/spouses aboard the Titanic
- `Parch`: Number of parents/children aboard the Titanic
- `Ticket`: Ticket number
- `Fare`: Ticket price
- `Cabin`: Cabin number
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Project Steps

1. **Data Loading and Inspection**:
   - Loaded the Titanic dataset and performed basic data exploration to understand the structure of the data.
   - Inspected data types and checked for missing values.

2. **Data Preprocessing**:
   - Dropped irrelevant columns such as `PassengerId`, `Name`, and `Ticket`.
   - Handled missing values in columns like `Age` and `Embarked`.
   - Applied one-hot encoding to categorical features like `Sex`, `Pclass`, `SibSp`, `Parch`, and `Embarked`.

3. **Feature Engineering**:
   - Converted categorical variables into numerical representations using one-hot encoding.
   - Prepared the final dataset (`X` and `y`), where `X` contains the features and `y` contains the target variable (`Survived`).

4. **Model Training**:
   - Split the dataset into training and testing sets.
   - Trained multiple machine learning models, including the `AdaBoostClassifier` with a base classifier (`RandomForestClassifier`).
   - Evaluated model accuracy using the testing set.

5. **Model Evaluation**:
   - The model achieved an accuracy of approximately **83.58%** on the test data.

## Technologies Used

- Python
- Pandas
- NumPy
- scikit-learn
- Matplotlib (for visualization)
