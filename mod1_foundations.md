# Lectures:


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
$$ \hat Y = \hat f (X)$$
* $\hat Y$: Estimate for $Y$
* $\hat f$: estimate of the true function $f$
* $X$: Predictor variables

  _Should we add something on irreducible vs reducible error?_

**Inference** - Understanding the relationship between $X$ and $Y$.
### 2.1.2: How do we estiamte $f$?
## Types of Learning

## Parametric vs. Non-Parametric Models

## Bias-Variance Trade-Off

## Model Accuracy and Performance

## Classification Problems

## Regression Problems
