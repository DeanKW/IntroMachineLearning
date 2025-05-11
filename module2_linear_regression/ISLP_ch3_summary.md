# Chapter 3 Summary: Linear Regression
Linear regression (yes, the one from middle or high school) may seem boring and not worth your time, but it is!  It
is widely used and many fancier models are generalizations or extensions of linear regression.  So seriously, this is
important.
## 3.1 Simple Linear Regression
**Simple Linear Regression** assumes that the response variable, $Y$ has a linear relationship to a single predictor
variable $X$.
$$
\begin{equation*}
Y \approx \beta_0 + \beta_1 X
\end{equation*}
$$

> [!NOTE] This is the same relationship as $y=mx+b$ you likely remember from school. \
> $\beta_0$ represents the intercept, $b$ while $\beta_1$ represents the slope, $m$. \
> In the future, we will use this same notation when $Y$ and $X$ are vectors, usually writing them bolded
> $\mathbf{Y} \approx \beta_0 + \beta_1 \mathbf{X}$

$\beta_0$ and $\beta_1$ are referred to as the **coefficients** or **parameters**. \
We will use our training data to estimate these parameters and then indicate and reprsent our **model** as
$$
\begin{equation*}
\hat Y \approx \hat \beta_0 + \hat \beta_1 X
\end{equation*}
$$
> [!NOTE] We call this "hat notation."  In statistics, an hat over something indicates it's either an 
> [estimator](https://en.wikipedia.org/wiki/Estimator) or an estimated value

### 3.1.1 Estimating the Coefficients
Since we do not know the true relationship between $X$ and $Y$, we use the training data to estimate $\beta_0$ and 
$\beta_1$
> [!NOTE] Just like you did in middle/high school when calculating the line of best fit

We will use **least squares** as the criteria to determine what values to use for our parameters, $\beta_0$ and $\beta_1$.

The $i$<sup>th</sup> **residual** is the difference between the $i$<sup>th</sup> response variable and our prediction for
that variable
$$
e_i = y_i - \hat y_i
$$

The **residual sum of squares** is defined

$$
\begin{align*}
\text{RSS} &= e_1^2 + e_2^2 + \cdots + e_n^2 \\
&= (y_1 - \hat \beta_0 - \hat \beta_1 x_1)^2 + (y_2 - \hat \beta_0 - \hat \beta_1 x_2)^2  + \cdots + (y_n - \hat \beta_0 - \hat \beta_1 x_n)^2 
\end{align*}
$$

The parameters can be calculated as:

$$
\hat \beta_1 = \frac{\sum_{i=1}^n(x_i - \bar x)(y_i-\bar y)}{\sum_{i=1}^n(x_i - \bar xx)^2}\\
\hat \beta_0 = \bar y - \hat \beta_1 \bar x
$$
where $\bar y$ and $\bar x$ are the sample means.  $\bar y = \frac{1}{n}\sum_{i=1}^n y_i$ and $\bar x = \frac{1}{n}\sum_{i=1}^n x_i$ 
### 3.1.2 Assessing the Accuracy of the Coefficient Estimates
#### Standard Error
Standard error tells us the average amount that an estimate differs from the actual value.

$$
\text{Var}(\hat \mu) = \text{SE}(\hat \mu)^2 = \frac{\sigma^2}{n}
$$

$$
\text{SE}(\hat \beta_0)^2 = \sigma^2 \left[ \frac{1}{n} + \frac{\bar x ^2}{\sum_{i=1}^n (x_i - \bar x)^2} \right]
$$

$$
\text{SE}(\hat \beta_1)^2 = \frac{\sigma^2}{\sum_{i=1}^n (x_i - \bar x)^2}
$$

where $\sigma^2 = \text{Var}(\epsilon)$  While we generally don't know $\sigma^2$, it can be estimated from the data.  
The estimate of $\sigma$ is called **residual standard error**
$$
\sigma = \text{RSE} = \sqrt{\frac{\text{RSS}}{n-2}}
$$
#### Confidence Intervals
Standard errors can be used to compute **confidence intervals**.  The 95% confidence interval for $\beta_0$ and $\beta_1$
are approximately:
$$
\hat \beta_0 \pm 2 \cdot \text{SE}(\hat \beta_0)\\
\hat \beta_1 \pm 2 \cdot \text{SE}(\hat \beta_1)
$$
This means there is approximately a 95% chance that the interval 
$$
\left[\beta_0 - 2 \cdot \text{SE}(\hat \beta_0), \beta_0 + 2 \cdot \text{SE}(\hat \beta_0)\right]
$$
contains the true value for $\beta_0$.  **NOTE: This is an incorrect interpretation of a confidence interval
, but it is what the book writes.  Please see the warning below**

> [!NOTE]
> 1.96 is closer to the correct value than 2.  This value comes from the Z-score value for a 97.5% quantile of a
> t-distribution.  You are likely to see these in any statistics class.

> [!WARNING]
> A 95% confidence interval does **NOT** mean we are 95% confident that the true parameters lies within that range. \
> What it really means is that we sampled the data 100 times, each time calculating the parameter and confidence interval
> 95% of those confidence intervals would contain the true value of the parameter. \
> It's a small distinction, but I wanted to make it, even if the book did not. \
> That said, it's generally okay to say we're 95% confidence the true value is in the interval, even if it's incorrect.
> In pure statistics, the distinction is generally considered

## 3.2 Multiple Linear Regression
### 3.2.1 Estimating the Regression Coefficients
### 3.2.2 Some Important Questions
## 3.3 Other Considerations in the Regression MOdel
## 3.4 The Marketing Plan
## 3.5 Comparison of Linear Regression with K-Nearest Neighbors