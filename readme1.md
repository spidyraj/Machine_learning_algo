# Assignment 4: Logistic Regression from Scratch

This repository contains an implementation of logistic regression from scratch using Python. The project was developed as part of an assignment and demonstrates the complete workflow from data preprocessing to model evaluation without relying on high-level machine learning libraries like scikit-learn, TensorFlow, or PyTorch.

## Project Overview

- **Data Loading and Preprocessing:**
  - The independent variables (`X`) and dependent variable (`Y`) are loaded from CSV files.
  - The features in `X` are normalized to improve convergence during training.

- **Model Implementation:**
  - **Sigmoid Function:** Used to map the linear combination of inputs to probabilities.
  - **Cost Function:** Binary cross-entropy loss is implemented to measure the error between predictions and actual labels.
  - **Batch Gradient Descent:** Parameters (θ) are updated iteratively to minimize the cost function.

- **Visualization:**
  - **Cost vs. Iteration Plot:** Demonstrates the decrease in cost over training iterations.
  - **Decision Boundary Plot:** Shows the data points along with the linear decision boundary computed by the model.
  - **Learning Rate Comparison:** Compares cost curves for learning rates of 0.1 and 5 over 100 iterations.

- **Evaluation:**
  - Predictions are made using the trained model.
  - A confusion matrix is generated, and performance metrics such as accuracy, precision, recall, and F1-score are calculated.

## Files in the Repository

- **`logistic_regression.ipynb`**: Jupyter/Google Colab notebook with the full code implementation.
- **`logisticX (1) - logisticX (1).csv`**: CSV file containing the independent variables.
- **`logisticY - logisticY.csv`**: CSV file containing the dependent variable.
- **`README.md`**: This file.

## How to Run

1. **Using Google Colab:**
   - Open the `logistic_regression.ipynb` notebook in Google Colab.
   - Upload the CSV files (`logisticX (1) - logisticX (1).csv` and `logisticY - logisticY.csv`) to the Colab environment.
   - Run the notebook cells sequentially to observe the outputs, plots, and evaluation metrics.

2. **Locally:**
   - Clone this repository.
   - Ensure that Python 3.x is installed along with `numpy`, `pandas`, and `matplotlib`.
   - Open and run the notebook using Jupyter Notebook or another compatible environment.

## Experimental Results

- **Final Model:**  
  The model trained with a learning rate of 0.1 converges to a final cost value, and the learned parameters define a decision boundary that separates the classes.

- **Plots:**
  - The cost function plot demonstrates steady convergence.
  - The decision boundary plot visually confirms the model's classification performance.
  - A comparison of learning rates shows that a higher rate (α = 5) may lead to unstable convergence compared to α = 0.1.

- **Evaluation Metrics:**  
  A confusion matrix and derived metrics (accuracy, precision, recall, F1-score) are provided to evaluate the model's performance.

