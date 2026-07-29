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

<img width="713" height="479" alt="image" src="https://github.com/user-attachments/assets/0b5a43b8-8743-449a-8745-a943670009ae" />

 
- Linear Regression fit

<img width="713" height="479" alt="image" src="https://github.com/user-attachments/assets/481d9160-4453-4400-808d-d4d368614e88" />


- Neural Network fit

<img width="713" height="479" alt="image" src="https://github.com/user-attachments/assets/6aae0878-0c73-47ca-b25a-fead79d91ecb" />


- Linear Regression loss curve

<img width="710" height="479" alt="image" src="https://github.com/user-attachments/assets/fc8baa30-20ad-4215-a06e-67a096640f48" />


- Neural Network loss curve

<img width="699" height="479" alt="image" src="https://github.com/user-attachments/assets/53ec9ad5-6eba-494d-91e6-628d69d2f272" />


- Learning rate comparison

<img width="777" height="556" alt="image" src="https://github.com/user-attachments/assets/ab4028a5-993f-4e21-9b43-64dddfb921ad" />


- Linear Regression vs Neural Network prediction comparison

<img width="868" height="556" alt="image" src="https://github.com/user-attachments/assets/33a0fd7a-6747-4323-b4ea-385386bdb5fe" />


- Training loss comparison

<img width="777" height="556" alt="image" src="https://github.com/user-attachments/assets/cfc3c72c-f8b8-4ca8-98c3-02e5faeda868" />



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
cd gradient-based-learning
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
