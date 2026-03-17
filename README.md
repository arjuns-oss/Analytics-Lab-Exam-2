Predictive Analytics Lab Exam – 2
Binary Classification Analysis
Overview

This project performs a binary classification task using a dataset with two numerical features. The goal is to explore the dataset, build classification models, and visualize how the model separates the classes.

The analysis includes:

Exploratory Data Analysis (EDA)

Data preprocessing

Model building

Decision boundary visualization

Model evaluation

Dataset

The dataset used for this project contains three columns:

Column	Description
Feature1	First numerical feature
Feature2	Second numerical feature
Target	Binary class label (Yes / No)

The Target variable represents the class that the model tries to predict.

Exploratory Data Analysis (EDA)

EDA is performed to understand the dataset and identify patterns.

The following steps were carried out:

1. Display Dataset

The first few rows of the dataset were displayed using:

data.head()
2. Dataset Information

Information about data types and number of entries was obtained using:

data.info()
3. Statistical Summary

Statistical summary of numerical features was obtained using:

data.describe()
4. Missing Value Check

To ensure data quality, missing values were checked using:

data.isnull().sum()
5. Class Distribution

A count plot was used to visualize the distribution of classes in the dataset.

sns.countplot(x='Target', data=data)

This helps understand whether the dataset is balanced or imbalanced.

6. Feature Relationship Visualization

A scatter plot was created to observe the relationship between the two features.

sns.scatterplot(x='Feature1', y='Feature2', hue='Target', data=data)

This plot helps visualize how the classes are distributed in the feature space.

Data Preprocessing

Before building models, the following preprocessing steps were applied:

Handling missing values

Converting target labels into numeric values

Splitting the dataset into training and testing sets

Feature scaling (for some models)

Classification Models

Two classification algorithms were used in this project.

1. Logistic Regression

Logistic Regression is a linear classification algorithm that predicts probabilities and separates classes using a linear boundary.

Steps performed:

Train the model using training data

Predict labels on test data

Evaluate model performance

2. Decision Tree Classifier

A Decision Tree model was also used to capture nonlinear patterns in the data.

Advantages of Decision Tree:

Handles nonlinear boundaries

Easy to visualize

Interpretable model

Decision Boundary Visualization

To understand how the classifier separates the classes, a decision boundary plot was generated.

Steps used:

Create a mesh grid over the feature space

Predict class labels for each grid point

Plot contour regions representing predicted classes

Overlay original dataset points

This visualization shows how the model divides the feature space into different class regions.

Technologies Used

The following libraries were used in this project:

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Jupyter Notebook

Project Structure
Predictive-Analytics-Lab-Exam-2
│
├── Lab2.ipynb
├── Lab_Exam_binary_classification_dataset.csv
└── README.md
Conclusion

This project demonstrates the complete workflow of a machine learning classification task, including:

Data exploration

Data preprocessing

Model training

Model evaluation

Visualization of decision boundaries

The results show how different models classify the dataset and how decision boundaries help in understanding model behavior.
