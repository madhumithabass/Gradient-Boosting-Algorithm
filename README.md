# Gradient Boosting Algorithms

## Overview

Gradient Boosting is an **ensemble machine learning technique** that combines multiple weak learners, usually **Decision Trees**, to build a strong predictive model.

Unlike Bagging methods such as Random Forest, where trees are built independently, **Boosting builds models sequentially**. Each new model tries to correct the errors made by the previous models.

This README covers:

* Gradient Descent
* Gradient Boosting
* Extreme Gradient Boosting (XGBoost)
* Light Gradient Boosting (LightGBM)
* Advantages and disadvantages
* Basic implementation and working of the code

---

# 1. Gradient Descent

## 📖 Theory

Gradient Descent is an **optimization algorithm** used to minimize a loss or cost function.

The goal of machine learning is to find model parameters that produce the smallest possible error.

Gradient Descent repeatedly updates the model parameters in the direction that reduces the loss.

### Basic Idea

1. Start with initial parameter values.
2. Calculate the error.
3. Calculate the gradient of the loss function.
4. Move the parameters in the opposite direction of the gradient.
5. Repeat until the loss is minimized.

### Parameter Update

```text
New Parameter = Old Parameter - Learning Rate × Gradient
```

The **learning rate** controls how large each update is.

* Small learning rate → slower learning but more controlled
* Large learning rate → faster learning but may overshoot the minimum

---

## 🔄 How Gradient Descent Works

Suppose a model has a high prediction error.

Gradient Descent calculates the direction in which the error decreases and updates the model accordingly.

```text
Initial Model
     ↓
Calculate Loss
     ↓
Calculate Gradient
     ↓
Update Parameters
     ↓
Calculate Loss Again
     ↓
Repeat
     ↓
Minimum Loss
```

---

## ✅ Advantages of Gradient Descent

* Simple and widely used optimization technique
* Works well with large datasets
* Can optimize complex models
* Used in Linear Regression, Logistic Regression, Neural Networks, and many other algorithms

## ❌ Disadvantages of Gradient Descent

* Can be slow with a very small learning rate
* A very large learning rate can cause
