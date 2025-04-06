# Fuel Efficiency Classification Using the Auto Dataset
This project focuses on building a classification model to predict whether a car has high or low fuel efficiency based on various technical specifications from the Auto dataset.

## Objective
The primary goal of this project is to compare the performance of several classification models in predicting whether a car's miles per gallon (mpg) is above or below the median value. A new binary variable, mpg01, is created to serve as the target:

mpg01 = 1 if the car's mpg is greater than the median

mpg01 = 0 if the car's mpg is less than or equal to the median

By applying and evaluating multiple models, we aim to identify which algorithm performs best for this specific classification problem.

## Dataset Overview
The Auto dataset includes the following features:

mpg: Miles per gallon (fuel efficiency)

cylinders: Number of engine cylinders

displacement: Engine displacement (in cubic inches)

horsepower: Engine horsepower

weight: Vehicle weight

acceleration: Time to accelerate from 0 to 60 mph

year: Model year

origin: Origin of the car (e.g., USA, Europe, Asia)

name: Car name (excluded from modeling due to high cardinality)

## Data Preparation
Created the binary target variable mpg01 based on the median of mpg.

Combined mpg01 with the rest of the dataset to create a unified DataFrame for modeling.

Applied standard preprocessing steps: handling missing values, converting categorical data, and normalizing where appropriate.

Detected and removed outliers using the IQR (Interquartile Range) method to eliminate extreme values that could negatively impact model performance.

## Models Compared
The following classification algorithms were implemented and compared:

Logistic Regression

K-Nearest Neighbors (KNN)

QDA (QuadraticDiscriminantAnalysis)

LDA (LinearDiscriminantAnalysis)

## Model Evaluation
Each model’s performance was evaluated using:

Accuracy

Precision & Recall

Confusion Matrix

F1_score

## Installation & Setup

Ensure you have Python installed along with the required libraries.

Install dependencies using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn

