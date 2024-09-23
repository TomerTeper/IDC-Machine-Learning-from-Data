
# HW2: Decision Tree Classifier Implementation

## Overview
This project implements a basic decision tree algorithm in Python. It includes functions for calculating decision tree metrics like Gini impurity and entropy, and defines a class-based structure for building and working with decision trees.

## Contents

### 1. **Warm-up: Object-Oriented Programming in Python**
   The notebook starts with a brief introduction to Python classes and object-oriented programming (OOP), which serves as a foundation for implementing the decision tree.

   - Example of a simple `Node` class with children.
   - Reference link to Python OOP tutorials.

### 2. **Functions for Decision Tree**
   The core functions include:
   - **`calc_gini(data)`**: Calculates the Gini impurity for a dataset.
   - **`calc_entropy(data)`**: Calculates the entropy for a dataset, often used for classification tasks.
   - **`count_nodes(node)`**: Recursively counts the number of nodes in a decision tree.

### 3. **Class Definitions for Decision Trees**
   The notebook defines several key classes:
   - **`DecisionNode`**: This class represents a node in the decision tree. It includes methods to calculate predictions, handle child nodes, and determine terminal nodes.
   - **`DecisionTree`**: This class orchestrates the overall construction of the decision tree, including training and testing.

### 4. **Implementation of Decision Tree**
   - The decision tree is implemented as a recursive structure, where each node splits the data based on the feature that maximizes the information gain or minimizes the Gini impurity.
   - Optionally, the decision tree can be pruned or limited in depth.

### 5. **Evaluation**
   - Methods are provided to evaluate the accuracy of the decision tree on training and test datasets.
   - Includes functionality to visualize the tree structure.


