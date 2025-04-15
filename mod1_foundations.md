# Lectures:
* [Statistical Learning 1.1: Opening Remarks](https://www.youtube.com/watch?v=LvySJGj-88U&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=1)
  * [Statistical Learning: 8 Years Later (Second Edition of the Course)](https://www.youtube.com/watch?v=9vlDVxG4ulA&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=2)

* [Statistical Learning 1.2: Examples and Framework](https://www.youtube.com/watch?v=B9s8rpdNxU0&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=4)
* [Statistical learning 2.1: Introduction to Regression Models](https://www.youtube.com/watch?v=ox0cKk7h4o0&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=5)
* [Statistical Learning 2.2: Dimensionality and Structured Models](https://www.youtube.com/watch?v=uFwbrdvrAJs&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=6)
* [Statistical Learning 2.3: Model Selection and Bias Variance Tradeoff](https://www.youtube.com/watch?v=pvcEQfcO3pk&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=7)
* [Statistical Learning 2.4: Classification](https://www.youtube.com/watch?v=BMJQ3LQ_QKU&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=8)

## Labs
* [Statistical Learning I: Introducing Jonathan - Third Edition of the Course | 2023](https://www.youtube.com/watch?v=Igd5srPxZfU&list=PLoROMvodv4rNHU1-iPeDRH-J0cL-CrIda&index=1)
* [Statistical Learning: 2.Py Setting Up Python | 2023](https://www.youtube.com/watch?v=RelOJOIKaTk&list=PLoROMvodv4rNHU1-iPeDRH-J0cL-CrIda&index=2)
* [Statistical Learning: 2.Py Data Types, Arrays, and Basics | 2023](https://www.youtube.com/watch?v=Cv1sx_HNRHM&list=PLoROMvodv4rNHU1-iPeDRH-J0cL-CrIda&index=3)

  
# Readings:
* _Introduction to Statistical Learning_: Chapter 1
* _Introduction to Statistical Learning_: Chapter 2

# Goals
* Understand classification vs. regression
* Understand the Bias-Variance Tradeoff (seriously, this will come up again and again.  It's a cornerstone in ML)
* Be able to run python and jupyter

## Things to Think About:
* When might a less accurate model that is more easily understood be more appropriate?
* What is overfitting?  Are we more likely to overfit our data with a more complex and less easily understood model?
* What's the relationship between the bias-variance tradeoff, overfitting, and model generalizability?
* What does it mean for a machine to learn?
* When can we think of $f$ as a black box and when might we need to understand it?

# Lab:
[Introduction to Python](https://github.com/intro-stat-learning/ISLP_labs/blob/stable/Ch02-statlearn-lab.ipynb)

## Assignments:

# Chapter 2 Summary: Statistical Learning
## 2.1: What is Statistical Learning?
**Statistical Learning** is a set of tools for estimating a function, $f$, that connects input variables $X$ and output variables $Y$.  We estimate $f$ because we do not (and often can not) know the true relationship.

**Goal:** Given data $(X_1, Y_1), (X_2, Y_2), ..., (X_n, Y_n)$, where:
* $X$: Predictors/Independent Variables/features
* $Y$: Response/Dependent Variable
* $\epsilon$: Irreducible error
  Estimate he function $f$ that relates $X$ and $Y$:
  $$Y = f(X) + \epsilon$$

### 2.1.1: Why Estimate $f$?
Two primary reasons to estimate $f$: **prediction** and **inference**

**Prediction** - Using input variables $X$ to predict an output variable $Y$

$$\hat Y = \hat f (X)$$
* $\hat Y$: Estimate for $Y$
* $\hat f$: estimate of the true function $f$
* $X$: Predictor variables

  _Should we add something on irreducible vs reducible error?_

**Inference** - Understanding the relationship between $X$ and $Y$.
### 2.1.2: How do we estimate $f$?
## Types of Learning

## Parametric vs. Non-Parametric Models

## Bias-Variance Trade-Off

## Model Accuracy and Performance

## Classification Problems

## Regression Problems
