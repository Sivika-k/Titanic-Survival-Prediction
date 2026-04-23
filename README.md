Titanic Survival Prediction using Machine Learning

Project Overview

The Titanic Survival Prediction project aims to build a machine learning model that can predict whether a passenger survived or not during the Titanic disaster. This is one of the most popular beginner-friendly datasets in data science and is widely used to understand classification problems.

The dataset contains detailed information about passengers such as their age, gender, ticket class, fare paid, family members onboard, and port of embarkation. By analyzing these features, the model learns patterns that influence survival probability.

Objective

The primary objective of this project is to:

* Develop a classification model to predict passenger survival
* Perform data preprocessing and cleaning
* Apply machine learning algorithms effectively
* Evaluate model performance using standard metrics

Dataset Description

 Features:

* **Pclass** → Passenger class (1 = First, 2 = Second, 3 = Third)
* **Sex** → Gender of the passenger
* **Age** → Age of the passenger
* **SibSp** → Number of siblings/spouses aboard
* **Parch** → Number of parents/children aboard
* **Fare** → Ticket fare
* **Embarked** → Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

Target Variable:

* **Survived**

  * 0 → Did not survive
  * 1 → Survived

Technologies Used

* **Python**
* **Pandas**
* **Scikit-learn**

Machine Learning Model

This project uses the **Random Forest Classifier**, an ensemble learning algorithm that builds multiple decision trees and combines their outputs to improve prediction accuracy and reduce overfitting.

Methodology

1. Data Loading

The dataset is loaded using the Pandas library.

2. Data Cleaning

Removed unnecessary columns:

* PassengerId
* Name
* Ticket
* Cabin

3. Handling Missing Values

* Missing values in **Age** are filled using the median value
* Missing values in **Embarked** are filled using the mode

4. Data Encoding

Categorical variables like **Sex** and **Embarked** are converted into numerical values using Label Encoding

5. Feature Selection

Input features (X) and target variable (y) are separated

6. Train-Test Split

Dataset is split into training (80%) and testing (20%) sets

7. Model Training

Random Forest Classifier is trained using training data

8. Model Prediction

Predictions are made on the test dataset

9. Model Evaluation

Evaluated using:

* Accuracy Score
* Precision
* Recall
* F1-score

Results and Performance

Overall Accuracy:

**82.12%**

Classification Metrics:

* **Precision (Survived = 1):** 0.81
* **Recall (Survived = 1):** 0.74
* **F1-Score:** 0.77

Detailed Classification Report:

              precision    recall  f1-score   support

           0       0.83      0.88      0.85       105
           1       0.81      0.74      0.77        74

    accuracy                           0.82       179
   macro avg       0.82      0.81      0.81       179
weighted avg       0.82      0.82      0.82       179

Interpretation:

* The model predicts **non-survivors** more accurately than survivors
* Overall performance is balanced and reliable
* Random Forest effectively handles feature relationships

Result:

This project demonstrates how machine learning can be applied to a real-world classification problem. The Random Forest model achieved an accuracy of approximately **82%**, making it a strong baseline model.

Author:

**Sivika K**
