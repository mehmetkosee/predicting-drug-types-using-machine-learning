# Drug Classification using Machine Learning

This project demonstrates how to predict the type of drug appropriate for a patient based on their health metrics using various machine learning algorithms. The analysis utilizes the Drug Classification dataset.

## Overview

The goal of this project is to build a classifier that can accurately predict the target drug (DrugY, drugA, drugB, drugC, or drugX) given features such as age, sex, blood pressure, cholesterol levels, and the sodium-to-potassium ratio in the blood.

## Dataset

The dataset used is the "Drug Classification" dataset. It contains patient information with the following attributes:
* Age
* Sex
* Blood Pressure (BP)
* Cholesterol
* Na_to_K (Sodium to Potassium Ratio)
* Drug (Target Variable)

## Methodology

The project workflow includes the following steps:
1.  **Data Preprocessing**: Handling categorical data using One-Hot Encoding and Label Encoding.
2.  **Exploratory Data Analysis (EDA)**: Visualizing feature distributions and relationships.
3.  **Model Training**: Implementing multiple classification algorithms.
4.  **Hyperparameter Tuning**: Using GridSearchCV to find optimal parameters.
5.  **Evaluation**: Comparing models based on accuracy, precision, recall, and F1-score.

## Technologies Used

* Python 3
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

## Models and Performance

The following models were trained and evaluated:

1.  **Logistic Regression**: Achieved approximately 78% accuracy.
2.  **Random Forest Classifier**: Achieved approximately 98% accuracy.
3.  **Decision Tree Classifier**: Achieved approximately 98% accuracy.
4.  **Support Vector Machine (SVM)**: Achieved approximately 95% accuracy after scaling and hyperparameter tuning.

Feature importance analysis showed that the Sodium-to-Potassium ratio (Na_to_K) is the most significant factor in determining the drug type.

## How to Run

1.  Clone the repository.
2.  Install the required libraries:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
3.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook predicting-drug-types-using-machine-learning.ipynb
    ```
