# Red Wine Quality Prediction

This repository contains a machine learning project focused on predicting the quality of red wine using Logistic Regression and Random Forest Classifier algorithms. The project leverages a dataset containing various physicochemical features related to red wines to classify their quality into three categories.

## Introduction

Predicting the quality of wine is a common task in the field of machine learning, with applications in the food and beverage industry. This project aims to build effective predictive models that can classify wine quality based on various features. Logistic Regression and Random Forest algorithms were chosen for their robustness and ability to handle different types of data.

By the end of this project, we expect the models to classify wine quality with reasonable accuracy, while providing insights into the factors that influence the final quality rating.

## Dataset Overview

You can find the dataset used in this project above ( winequality-red.csv ) . It contains various attributes of red wine samples along with their quality ratings, which are classified into three categories:
- Low Quality (1)
- Medium Quality (2)
- High Quality (3)

The dataset includes features such as acidity, sugar content, sulfur dioxide levels, and alcohol content.

## Preprocessing Steps

To prepare the data for modeling, several preprocessing steps were applied:

- **Handling Missing Values**: The dataset was checked for missing values and handled accordingly to ensure a clean dataset for modeling.
  
- **Label Binarization**: The quality ratings were binned into three classes to facilitate classification.

- **Feature Selection**: The relevant features were selected for model training, and any unnecessary columns were dropped.

- **Data Scaling**: The features were standardized using `StandardScaler` to ensure that they are on a similar scale, which is particularly beneficial for Logistic Regression.

## Algorithms Used

- **Logistic Regression**: This model was implemented to predict wine quality. Logistic Regression is a statistical method that models the relationship between the dependent variable (quality) and one or more independent variables (features).

- **Random Forest Classifier**: This algorithm creates multiple decision trees during training and merges their results to produce more accurate and stable predictions. It is particularly useful in dealing with complex datasets and reducing variance, thereby minimizing overfitting.

The models were trained on the training data, and their performance was evaluated using accuracy scores.

## Installation

To run this project locally, ensure you have Python installed along with the necessary libraries. You can install the required dependencies by running:

```bash
pip install pandas scikit-learn numpy matplotlib seaborn
```

## Usage
1. Download the Red Wine Quality dataset and place it in the project directory.

2. Run the Python script code.py to preprocess the data, train the models, and generate predictions:

```bash
python wine_quality_model.py
```
The output will include accuracy scores for both Logistic Regression and Random Forest models.

## Results
After training and evaluating the models, the following performance metrics were achieved:

* Logistic Regression Accuracy: 0.98125
* Random Forest Classifier Accuracy: 0.978125
