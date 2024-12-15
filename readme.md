# Decision Trees and Ensemble Methods from Scratch

This repository contains implementations of various tree-based machine learning algorithms and ensemble methods from first principles. It aims to provide a deeper understanding of how decision trees, random forests, AdaBoost, and gradient boosting machines (GBMs) work under the hood. Additionally, it showcases the usage of popular gradient boosting frameworks such as XGBoost, LightGBM, and CatBoost for classification, regression, and ranking tasks.
# [Video link](https://youtu.be/e9Er4_LkXdI)

## Table of Contents

- [Overview](#overview)
- [Implemented Algorithms](#implemented-algorithms)
  - [Decision Tree From Scratch](#decision-tree-from-scratch)
  - [Random Forest From Scratch](#random-forest-from-scratch)
  - [AdaBoost From Scratch](#adaboost-from-scratch)
  - [Gradient Boosting (GBM) From Scratch](#gradient-boosting-gbm-from-scratch)
- [Demonstrations](#demonstrations)
  - [Classification with Decision Trees and Ensembles](#classification-with-decision-trees-and-ensembles)
  - [Regression with Ensemble Methods](#regression-with-ensemble-methods)
- [Advanced GBM Frameworks](#advanced-gbm-frameworks)
  - [XGBoost, LightGBM, and CatBoost for Classification](#xgboost-lightgbm-and-catboost-for-classification)
  - [XGBoost, LightGBM, and CatBoost for Regression](#xgboost-lightgbm-and-catboost-for-regression)
  - [Gradient Boosting Ranking Techniques](#gradient-boosting-ranking-techniques)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Notebooks](#running-the-notebooks)
- [Repository Structure](#repository-structure)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project is part of a machine learning assignment focusing on decision trees and ensemble methods. By implementing these algorithms from scratch, we gain a clear understanding of their core principles, including:

- How decision trees use impurity measures (e.g., Gini, entropy) to find optimal splits.
- The concept of bootstrapping and random feature selection in random forests.
- How AdaBoost iteratively adjusts sample weights to focus on harder cases.
- The logic behind gradient boosting, where models are added sequentially to correct residual errors of previous models.

We then compare our from-scratch implementations with well-known libraries and frameworks, giving insight into their performance, features, and ease of use.

## Implemented Algorithms

### Decision Tree From Scratch

- Implements ID3/CART-like logic for splitting nodes based on Gini or entropy.
- Provides stopping criteria (max depth, min samples, etc.).
- Demonstrates training and prediction on a simple dataset.
  
### Random Forest From Scratch

- Uses multiple decision trees trained on bootstrap samples of the data.
- Randomly selects a subset of features for splitting at each node.
- Aggregates predictions by majority vote (classification) or averaging (regression).
- Showcases improved robustness and generalization over a single decision tree.

### AdaBoost From Scratch

- Trains a series of weak learners (e.g., decision stumps) on weighted samples.
- Updates sample weights after each weak learner is added, emphasizing harder cases.
- Combines weak learners into a strong classifier with improved accuracy.

### Gradient Boosting (GBM) From Scratch

- Begins with an initial model (often the mean prediction for regression).
- Iteratively fits new models to the current residuals.
- Uses a learning rate to gradually improve the model’s predictive power.
- Demonstrates a flexible and powerful ensemble technique for both classification and regression.

## Demonstrations

### Classification with Decision Trees and Ensembles

- Evaluate accuracy on a known classification dataset (e.g., Iris, Wine).
- Compare the performance of a single decision tree with random forests, AdaBoost, and a GBM.

### Regression with Ensemble Methods

- Use a synthetic or real-world regression dataset.
- Show how gradient boosting reduces residual errors over iterations.
- Compare single-tree predictions to GBM predictions to highlight performance gains.

## Advanced GBM Frameworks

After gaining an in-depth understanding of the fundamentals, we leverage well-known libraries to:

### XGBoost, LightGBM, and CatBoost for Classification

- Train and compare these frameworks on a classification task.
- Explore feature importances, training speed, and accuracy.

### XGBoost, LightGBM, and CatBoost for Regression

- Apply these frameworks to a regression dataset.
- Evaluate predictions against ground truth and analyze errors.

### Gradient Boosting Ranking Techniques

- Optional: Show how to use LightGBM or XGBoost for ranking tasks if a suitable dataset is provided.
- Discuss parameter configurations for ranking and relevant evaluation metrics.

## Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook or Google Colab environment

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/decision-trees-ensemble-from-scratch.git
   cd decision-trees-ensemble-from-scratch
