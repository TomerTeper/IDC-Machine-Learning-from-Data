
# HW4: Logistic Regression, Bayes and EM

## Overview

This project implements several core machine learning techniques, focusing on both supervised and unsupervised learning. The key tasks covered include:

- **Feature Selection**: Identifying the most relevant features to improve model performance.
- **Logistic Regression**: A simple but effective binary classifier.
- **Cross Validation**: A robust evaluation method to assess model performance.
- **Expectation-Maximization (EM)**: A probabilistic algorithm used for clustering and density estimation.
- **Gaussian Mixture Models (GMM)**: An extension of the EM algorithm to model data with multiple Gaussian distributions.
- **Naive Bayes Classifier**: A fast and simple probabilistic classifier based on Bayes' Theorem.
- **Model Evaluation**: Techniques such as accuracy, precision, recall, and confusion matrices are used to assess model performance.

## Detailed Overview of Sections

### 1. Feature Selection

Feature selection is a critical step in building efficient machine learning models, as it helps reduce overfitting, speeds up training, and improves model performance. This section implements feature selection by applying methods such as:
- **Filter methods**: Selecting features based on statistical measures (e.g., correlation or chi-square test).
- **Wrapper methods**: Using model performance to select the best subset of features (e.g., recursive feature elimination).

### 2. Logistic Regression

Logistic Regression is implemented as a baseline classification model. It is useful for binary classification tasks, where the output is a probability of belonging to one of two classes.

- **Objective**: Fit a logistic model to the data and make predictions based on learned weights.
- **Key steps**:
  - Calculate the sigmoid function for prediction.
  - Optimize the weights using gradient descent to minimize the binary cross-entropy loss function.

### 3. Cross Validation

Cross validation is a technique used to evaluate model performance in a robust manner. Instead of relying on a single train-test split, this method splits the data into multiple folds and trains the model on different folds while testing on the remaining data.

- **k-Fold Cross Validation**: The dataset is divided into `k` subsets, and the model is trained `k` times, each time using a different subset as the test set and the remaining data for training.

### 4. Expectation-Maximization (EM) Algorithm

The EM algorithm is used for finding maximum likelihood estimates of parameters in probabilistic models with latent variables. This section applies the EM algorithm for clustering tasks, particularly focusing on Gaussian Mixture Models (GMM).

- **Initialization**: Set initial values for means, variances, and weights.
- **Expectation Step**: Calculate the responsibility for each data point.
- **Maximization Step**: Update the model parameters based on calculated responsibilities.

### 5. Gaussian Mixture Models (GMM)

GMM is an extension of the EM algorithm, which assumes that the data is generated from a mixture of several Gaussian distributions. This section provides the implementation of GMM for clustering tasks, allowing for soft classification (each point belongs to multiple clusters with a certain probability).

### 6. Naive Bayes Classifier

Naive Bayes is a simple yet effective probabilistic classifier based on Bayes' Theorem. It is particularly well-suited for text classification tasks and is implemented here as a fast baseline classifier for comparison.

### 7. Model Evaluation

This section covers various evaluation metrics and methods to assess the performance of the models:
- **Accuracy**: The proportion of correct predictions.
- **Precision**: The proportion of positive predictions that were correct.
- **Recall**: The proportion of actual positives that were correctly identified.
- **Confusion Matrix**: A table that visualizes the performance of the classification model by showing the true positives, false positives, true negatives, and false negatives.

