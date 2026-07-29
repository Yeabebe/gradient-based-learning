# Gradient-Based Learning: From Linear Regression to a One-Hidden-Layer Neural Network

## Overview

This project implements two supervised learning algorithms completely **from scratch** using only **NumPy** and **Matplotlib**. The objective is to demonstrate the mathematical foundations of gradient-based learning by manually deriving and implementing gradient descent and backpropagation without relying on machine learning frameworks or automatic differentiation.

The project was developed as part of the practical assignment:

> **Deriving and Implementing Gradient-Based Learning: From Linear Regression to a One-Hidden-Layer Neural Network**

---

## Objectives

- Derive gradients for Linear Regression using the chain rule.
- Implement Linear Regression from scratch.
- Derive backpropagation equations for a one-hidden-layer neural network.
- Implement forward propagation and manual backpropagation.
- Compare model performance on a nonlinear regression dataset.
- Investigate the effect of different learning rates on convergence.

---

## Features

- Linear Regression implemented from scratch
- One-Hidden-Layer Neural Network implemented from scratch
- Manual Gradient Descent optimization
- Manual Backpropagation (no autograd)
- Xavier weight initialization
- Hyperbolic Tangent (tanh) activation function
- Mean Squared Error (MSE) loss
- Synthetic nonlinear dataset generation
- Learning rate comparison
- Multiple visualization plots

---

## Project Structure

```text
gradient_learning.ipynb
README.md
requirements.txt
```

---

## Technologies Used

- Python 3
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

---

## Dataset

A synthetic nonlinear regression dataset is generated using:

\[
y = \sin(x) + \epsilon
\]

where

- \(x \in [-3,3]\)
- \(\epsilon\) is Gaussian noise.

This dataset was selected to clearly demonstrate the limitations of Linear Regression and the ability of neural networks to learn nonlinear relationships.

---

## Models Implemented

### 1. Linear Regression

Implemented completely from scratch.

Includes:

- Prediction function
- Mean Squared Error Loss
- Manual gradient computation
- Gradient Descent optimization
- Training loop

Prediction equation

\[
\hat y = wx+b
\]

---

### 2. One-Hidden-Layer Neural Network

Architecture

```text
Input
   │
Hidden Layer (16 neurons)
   │
tanh Activation
   │
Output Layer
   │
Prediction
```

Implemented components

- Xavier Initialization
- Forward Propagation
- Manual Backpropagation
- Gradient Descent
- MSE Loss

No machine learning libraries were used.

---

## Learning Rate Experiment

The neural network was trained using three different learning rates.

| Learning Rate | Purpose |
|---------------|----------|
| 0.001 | Slow convergence |
| 0.01 | Stable convergence |
| 0.1 | Faster updates with potential instability |

The convergence behavior of each configuration is visualized and compared.

---

## Visualizations

The notebook includes:

- Synthetic dataset visualization
- Linear Regression fit
- Neural Network fit
- Linear Regression loss curve
- Neural Network loss curve
- Learning rate comparison
- Linear Regression vs Neural Network prediction comparison
- Training loss comparison

---

## Results

The experiments demonstrate that:

- Linear Regression performs well only for linear relationships.
- A one-hidden-layer neural network successfully learns nonlinear patterns.
- Learning rate significantly influences convergence speed and training stability.
- Manual backpropagation produces effective parameter updates using the derived gradients.

Example final performance:

| Model | Mean Squared Error |
|--------|-------------------:|
| Linear Regression | 0.183468 |
| Neural Network | 0.034625 |

The neural network achieves substantially lower prediction error on the nonlinear dataset.

---

## Mathematical Concepts Covered

- Gradient-Based Learning
- Gradient Descent
- Mean Squared Error
- Chain Rule
- Multivariate Chain Rule
- Forward Propagation
- Backpropagation
- Weight Initialization
- Activation Functions
- Learning Rate Analysis

---

## Installation

Clone the repository

```bash
git clone https://github.com/Yeabebe/gradient-based-learning.git
```

Navigate to the project directory

```bash
cd your-repository
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

or open the notebook using Visual Studio Code or Google Colab.

---

## Requirements

```text
numpy
matplotlib
jupyter
ipykernel
```

---

## Learning Outcomes

This project demonstrates how modern neural networks are built from the fundamental principles of calculus and linear algebra.

By implementing every component manually, the project provides a deeper understanding of:

- Gradient computation
- Parameter optimization
- Backpropagation
- Neural network training
- The relationship between mathematical derivations and practical machine learning implementation

---

## Author

**Yeabsera Abebe**

AI Engineer 

---

## License

This project is intended for educational and academic purposes.
