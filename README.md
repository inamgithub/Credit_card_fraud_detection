# Credit_card_fraud_detection
Using Scikit-Learn and Snap ML


This repository contains code for building and evaluating two popular classification models, Decision Tree and Support Vector Machine, to recognize fraudulent credit card transactions.

## Introduction

In this project, we utilize a real dataset containing credit card transaction information from September 2013 by European cardholders. The objective is to train models that can accurately identify legitimate and fraudulent credit card transactions.

## Models

We build two classification models:

1. **Decision Tree**: A decision tree is a tree-like model that makes decisions based on asking a series of questions. It's particularly useful for understanding the decision-making process and handling non-linear relationships in the data.

2. **Support Vector Machine (SVM)**: SVM is a powerful algorithm for classification tasks. It tries to find the optimal hyperplane that best separates the different classes in the data.

## Data

The dataset used for training and evaluation contains information on credit card transactions. The target variable, 'Class,' indicates whether a transaction is fraudulent (1) or legitimate (0). Since fraudulent transactions are rare, the dataset is highly imbalanced, with only a small percentage being fraudulent.

## Usage

1. **Download the Dataset**: We use a real credit card fraud dataset from Kaggle. You can download the dataset using the `opendatasets` library. Make sure to install it using `pip install opendatasets`.

2. **Install Dependencies**: Ensure you have the required Python packages installed. You can use the `requirements.txt` file to install them using `pip install -r requirements.txt`.

3. **Data Analysis**: The `Data Analysis` section of the code provides insights into the dataset, its shape, target variable distribution, and more.

4. **Data Preprocessing**: Data preprocessing steps like feature scaling and normalization are important for model convergence. The code demonstrates how to prepare the data for training.

5. **Train/Test Split**: The dataset is split into training and testing sets using the `train_test_split` function from `scikit-learn`.

6. **Decision Tree Model**: We build a Decision Tree model using both Scikit-Learn and Snap ML. Snap ML is shown to provide significantly faster training times.

7. **Evaluate Decision Tree Model**: The models' performance is evaluated using the ROC-AUC score on the test data. The training speedup achieved by Snap ML is also highlighted.

8. **Support Vector Machine Model**: Similar to the Decision Tree, we build SVM models using both Scikit-Learn and Snap ML.

9. **Evaluate SVM Model**: The SVM models are evaluated using the ROC-AUC score and hinge loss metric.

## Conclusion

This project demonstrates the process of building, training, and evaluating classification models for fraud detection using a real-world credit card transaction dataset. The Decision Tree and Support Vector Machine models are compared, and the benefits of Snap ML in terms of training speed are highlighted. The code provides a clear outline of the steps involved, making it easy to understand and replicate the process.
