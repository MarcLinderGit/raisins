# Predicting Raisin Variety with Decision Trees and Logistic Regression

## Introduction

In this data analysis project, the goal is to predict the variety of raisins using machine learning models. The dataset used in this analysis contains various features related to raisin properties and is labeled with two classes: 'Kecimen' and 'Besni.' The project explores the use of Decision Tree Classifier and Logistic Regression models for classification tasks. Additionally, hyperparameter tuning techniques, such as Grid Search and Randomized Search, are utilized to optimize model performance.

Data source: [Raisin Dataset](https://www.muratkoklu.com/datasets/) by [Murat Koklu](https://www.kaggle.com/muratkokludataset)

## Methods and Objectives

This project follows a systematic approach to build and evaluate machine learning models for raisin variety prediction:

1. **Data Loading and Preprocessing**: The necessary libraries are imported, and the dataset is loaded. The 'Class' column, representing the raisin variety, is recoded into binary values (0 for 'Kecimen' and 1 for 'Besni') for classification purposes.

2. **Exploratory Data Analysis (EDA)**: An initial exploration of the dataset is conducted, including printing the dataset's head and summarizing key statistics. This step aids in understanding the dataset's structure and class distribution.

3. **Data Splitting**: The dataset is divided into training and testing sets using the `train_test_split` function to assess model performance on unseen data.

4. **Grid Search with Decision Tree Classifier**: A Decision Tree Classifier model is created, and hyperparameter tuning is performed using Grid Search. The tuned parameters include 'min_samples_split' and 'max_depth.' The best estimator and the model's accuracy on the test data are printed.

5. **Randomized Search with Logistic Regression**: A Logistic Regression model is defined, and Randomized Search is employed for hyperparameter tuning. 'penalty' and 'C' hyperparameters are explored using a distribution defined by the uniform function. The best score and the model's accuracy on the test data are printed.

6. **Results Summary**: The results of both hyperparameter tuning processes are summarized, including the best hyperparameters, best scores on the training data, and accuracy on the test data. This summary provides insights into the model's performance and the impact of hyperparameter optimization.

By following this approach, the project aims to identify the most suitable machine learning model and hyperparameters for accurately predicting raisin variety. It also assesses the effectiveness of different search strategies (Grid Search and Randomized Search) for hyperparameter tuning.

Let's proceed with the code and delve into the details of these methods.