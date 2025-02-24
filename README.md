# Machine_learning_algo
it cointains various types of ML algo.
# Linear Regression using Gradient Descent

## Overview
This project implements **Linear Regression** using **Batch Gradient Descent, Stochastic Gradient Descent (SGD), and Mini-Batch Gradient Descent**. It explores the effects of different learning rates and compares convergence behaviors. The cost function is optimized iteratively until convergence criteria are met.

## Dataset
- The dataset consists of two CSV files:
  - `linearX.csv`: Contains the input feature values.
  - `linearY.csv`: Contains the corresponding target values.

## Approach
1. **Data Loading and Preprocessing:**
   - Load `linearX.csv` and `linearY.csv`.
   - Normalize `X` using **Z-score normalization**.
   
2. **Batch Gradient Descent Implementation:**
   - Add a **bias term** to `X`.
   - Initialize **θ (parameters) to zero**.
   - Update `θ` iteratively using **gradient descent** with Mean Squared Error (MSE) as the cost function.
   - Convergence criteria: **Change in cost < 1e-5**.

3. **Cost Function vs Iteration Plot:**
   - Store cost values during training.
   - Plot cost function trend for the first **50 iterations**.

4. **Regression Line Fitting:**
   - Plot original dataset.
   - Overlay the **best-fit regression line** obtained from training.

5. **Effect of Different Learning Rates:**
   - Train models using `lr = 0.005`, `lr = 0.5`, and `lr = 5`.
   - Observe cost function behavior for each case.
   - Compare results for **slow convergence, optimal learning, and divergence**.

6. **Comparison of Gradient Descent Variants:**
   - Implement and compare **Batch GD, SGD, and Mini-Batch GD**.
   - Analyze cost function changes and convergence speed.

## Observations
- **Batch Gradient Descent:** Smooth convergence but computationally expensive.
- **Stochastic Gradient Descent (SGD):** Faster updates but fluctuating cost function.
- **Mini-Batch Gradient Descent:** Balanced approach with moderate stability and faster convergence.

## Requirements
- Python 3.x
- NumPy
- Pandas
- Matplotlib

## Usage
Run the script in a Python environment to:
- Train a linear regression model.
- Compare different learning rates.
- Visualize cost function trends and regression fit.

## Results
The project demonstrates how gradient descent optimizes the cost function and how different learning rates and optimization strategies impact convergence.
