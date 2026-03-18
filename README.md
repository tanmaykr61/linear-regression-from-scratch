# Linear Regression from Scratch (NumPy)

A from-scratch implementation of Linear Regression built entirely using NumPy.

---

## Overview

This notebook builds Linear Regression step by step, starting from the mathematical formulation to implementing gradient descent and evaluating performance.

---

## What’s covered

- Understanding the linear regression equation  
- Implementing predictions using NumPy  
- Writing the cost function (Mean Squared Error)  
- Gradient Descent from scratch  
- Training the model iteratively  
- Evaluating performance using R² score  
- Visualizing regression line and error  

---

## Model Architecture

This implementation follows the standard structure of a simple Linear Regression model:

- **Input Features (X):** Numerical input data used to make predictions  
- **Weights (W):** Coefficients assigned to each feature, learned during training  
- **Bias (b):** A constant term added to shift the prediction line  

The model predicts outputs using a linear equation:

$$
y = Wx + b
$$

---

### Training Process

- Predictions are made using the current values of weights and bias  
- The **Mean Squared Error (MSE)** is used as the cost function  
- **Gradient Descent** is applied to iteratively update parameters  
- Weights and bias are adjusted to minimize the error over time  

---

### Evaluation Metric (R² Score)

The model performance is evaluated using the **R² score**, which measures how well the model explains the variance in the data:

$$
R^2 = 1 - \frac{\sum (y_{\text{true}} - y_{\text{pred}})^2}{\sum (y_{\text{true}} - \bar{y})^2}
$$

where:

- $y_{\text{true}}$ = actual values  
- $y_{\text{pred}}$ = predicted values  
- $\bar{y}$ = mean of actual values  

An R² score closer to 1 indicates a better fit.

---

## Implementation Details

The model is implemented without external ML libraries:

- Pure NumPy for all computations  
- Manual gradient updates  
- No abstraction layers, everything is explicit  

---

## How to run

### 1. Install dependencies

```shell
pip install numpy matplotlib pandas
```

### 2. Run the notebook

```shell
jupyter notebook linear_regression_from_scratch.ipynb
```

### 3. Run all cells to train and visualize the model

---

## Results

The model learns to fit a line to the data and achieves a reasonable R² score.

---

## License

This project is open-source under the MIT License.

---