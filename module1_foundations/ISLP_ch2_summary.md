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

#### Parametric vs. Non-Parametric Models
##### Parametric
1. Assume some functional form for $f$.  This is choosing the model.  One example would be linear:
$$f(x) = \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \cdots + \beta_p X_p$$
2. Fit or train the model.  Use some procedure to estimate the parameters (in this case $\beta_0, \beta_1, \cdots \beta_p$).  That is to say, find values for the parameters such that
$$Y \approx  \beta_0 + \beta_1 X_1 + \beta_2 X_2 + \cdots + \beta_p X_p$$

In this example, we have simplified the problem of estimating $f$ down to fitting parameters $\beta_0, \beta_1, \cdots \beta_p$
* Too flexible a model leads to underfitting and poor predictions
* Too complex a model leads to overfitting
* Choosing a functional form that is very different from the true form of $f$ will result in poor results
##### Non-Parametric
* No explicit assumption about the functional form of $f$
* More flexible since no specific function shape, can fit many shapes
* Requires far more training data to accurately estimate $f$ since the problem isn't reduced to estimating parameters
* Easy to overfit to training data

#### Supervised vs. Unsupervised Learning
##### Supervised
* For each observation, we have the input measurements, $x_i$ and the output, $y_i$ is labeled
* Ex: Linear Regression, Classification
##### Unsupervised
* For each observation, we have the input measurements $x_i$, but there is no associated response, $y_i$
* Often seek to understand the relationship between variables or observations
* Ex: Clustering

#### Regression vs. Classification Problems
##### Regression
* The response ($Y$) is quantitative (a number)
* Ex: Predicting income or the value of a house
##### Classification
* The response ($Y$) is qualitative (a category or label)
* Attempting to predict what group something is in
* Ex: Is an email spam or not spam?

## 2.2: Assessing Model Accuracy
### 2.2.1 Measuring the Quality of Fit
When estimating the function $\hat f(x)$ we need to determine how well it predicts the response variable, $Y$.  The most common way of doing this is with the **Mean Squared Error (MSE)**
$$\text{MSE} = \frac{1}{n}\sum_{i=1}^{n}\left(y_i - \hat f(x_i) \right)^2 $$
* $y_i$ - actual value
* $\hat f(x_i)$ - predicted value
* $n$ - number of data points

MSE is computed using the training data, but we don't really care about how well it does on training data!  Far more interested in how it predicts new, unseen data!  So what we want to do is split our test data and training data and test them separately!

**Test error is what we really care about, not the training error**

* Flexible (complex) models fit the training data very well and thus have low training error
* They may not generalize well to the test data, which results in poor results.  We call this **overfitting**
### 2.2.2: The Bias-Variance Trade-Off
* **Bias** - the error from wrong assumptions in the model
    * Can think of this as error caused by simplifying a real-life problem into a much simpler model
* **Variance** - error from the model being sensitive to small changes in the training set
    * Can think of this as "how much would $\hat f$ change if trained on different data

* High bias - underfit (model too simple)
* High variance - overfit (model too complex)

$$\begin{align*}
\text{E}[\text{MSE}]&=\text{Variance}+ \text{Bias}^2 + \text{Irreducible Error}\\
\text{E}[y_0 - \hat{f}(x_0)]&=\text{Var}(\hat f(x_0))+ [\text{Bias}(\hat f(x_0))]^2 + \text{Var}(\epsilon)\\
\end{align*}$$

### 2.2.3: The classification Setting
#### The Bayes Classifier
#### K-Nearest Neighbor

# Key Takeaways
* The goal of statistical learning is to estimate the function $f$ that connects input variable $X$ to output variable $Y$
* There are trade-offs between:
    * bias and variance
    * interpretability and flexibility
* Supervised learning can be either **regression** (quantitative $Y$) or **classification** (qualitative $Y$)
* Model assessment (testing) should be on data that is reserved for testing, not what was used to train
