Please see our [Recommended order](#our-suggested-order) and our [Module Notes](ISLP_ch2_notes.pdf).

# Lectures:
* [Statistical Learning 1.1: Opening Remarks](https://www.youtube.com/watch?v=LvySJGj-88U&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=1)
  * [Statistical Learning: 8 Years Later (Second Edition of the Course)](https://www.youtube.com/watch?v=9vlDVxG4ulA&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=2)

* [Statistical Learning 1.2: Examples and Framework](https://www.youtube.com/watch?v=B9s8rpdNxU0&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=4)
* [Statistical learning 2.1: Introduction to Regression Models](https://www.youtube.com/watch?v=ox0cKk7h4o0&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=5)
* [Statistical Learning 2.2: Dimensionality and Structured Models](https://www.youtube.com/watch?v=uFwbrdvrAJs&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=6)
* [Statistical Learning 2.3: Model Selection and Bias Variance Tradeoff](https://www.youtube.com/watch?v=pvcEQfcO3pk&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=7)
* [Statistical Learning 2.4: Classification](https://www.youtube.com/watch?v=BMJQ3LQ_QKU&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=8)

## Lecture Slides
* [Chapter 1 Slides](https://hastie.su.domains/ISLR2/Slides/Ch1_Inroduction.pdf)
* [Chapter 2 Slides](https://hastie.su.domains/ISLR2/Slides/Ch2_Statistical_Learning.pdf)
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
    * When a model is overfit, it means it has learned not only the actual relationship between variables, but also the random noise (irreducible error)
* What's the relationship between the bias-variance tradeoff, overfitting, and model generalizability?
* What does it mean for a machine to learn?
* When can we think of $f$ as a black box and when might we need to understand it?

# Lab:
[Introduction to Python](https://github.com/intro-stat-learning/ISLP_labs/blob/stable/Ch02-statlearn-lab.ipynb)

## Assignments:

# Notes
* [Chapter 2 Summary: Statistical Learning Notes](ISLP_ch2_notes.pdf)


# Our Suggested Order
* Watch [Statistical Learning 1.1: Opening Remarks](https://www.youtube.com/watch?v=LvySJGj-88U&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=1)
* Watch [Statistical Learning: 8 Years Later (Second Edition of the Course)](https://www.youtube.com/watch?v=9vlDVxG4ulA&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=2)

* Watch [Statistical Learning 1.2: Examples and Framework](https://www.youtube.com/watch?v=B9s8rpdNxU0&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=4)
* Read ISLP chapter 1

* Watch [Statistical learning 2.1: Introduction to Regression Models](https://www.youtube.com/watch?v=ox0cKk7h4o0&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=5)

* Watch [Statistical Learning 2.2: Dimensionality and Structured Models](https://www.youtube.com/watch?v=uFwbrdvrAJs&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=6)
    * Note that the curse of dimensionality is mentioned in the lecture, but not in the book.  We will use outside resources to go over it after learning about K-Nearest Neighbor
    * Pay attention to the parsimony vs. black box portion.

* Read ISLP 2.1: What is Statistical Learning?
    * Yes, this is correct.  Watch both of the above videos first

* Read this [AWS Article on Overfitting](https://aws.amazon.com/what-is/overfitting/).
    * Note: It's fine if you don't understand the sections:
        * **How can you detect overfitting?**
        * **How can you prevent overfitting?**
    * Feel free to skip the final section **How can AWS minimize overfitting errors in your machine learning models?**

* Watch [Statistical Learning 2.3: Model Selection and Bias Variance Tradeoff](https://www.youtube.com/watch?v=pvcEQfcO3pk&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=7)
    * Pay extra attention to the Bias-Variance Tradeoff!

* Read ISLP 2.2: Assessing Model Accuracy
    * 2.2.1 Measuring the Quality of Fit
    * 2.2.2 The Bias-Variance Trade-Off

* Watch [Statistical Learning 2.4: Classification](https://www.youtube.com/watch?v=BMJQ3LQ_QKU&list=PLoROMvodv4rPP6braWoRt5UCXYZ71GZIQ&index=8)

* Read 2.2.3 The Classification Setting
* Set up [Python environment](#setting-up-your-python-environment)
* Depending on your python/matplotlib/numpy/pandas knowledge
    * Watch [Statistical Learning I: Introducing Jonathan - Third Edition of the Course | 2023](https://www.youtube.com/watch?v=Igd5srPxZfU&list=PLoROMvodv4rNHU1-iPeDRH-J0cL-CrIda&index=1)
    * Watch [Statistical Learning: 2.Py Setting Up Python | 2023](https://www.youtube.com/watch?v=RelOJOIKaTk&list=PLoROMvodv4rNHU1-iPeDRH-J0cL-CrIda&index=2)
    * Watch [Statistical Learning: 2.Py Data Types, Arrays, and Basics | 2023](https://www.youtube.com/watch?v=Cv1sx_HNRHM&list=PLoROMvodv4rNHU1-iPeDRH-J0cL-CrIda&index=3)
    * Lab: Section 2.3 in ISLP.  [Introduction to Python](https://github.com/intro-stat-learning/ISLP_labs/blob/stable/Ch02-statlearn-lab.ipynb)
    * Even if you are super familiar with python, matplotlib, numpy, and pandas, I'd suggest skimming the lab.
* TODO: Figure out what exercises to suggest
* TODO: Figure out what optional/deeper reading to suggest.
    * Stick to HOML or use something else? Raschka?  Why Machines learn?  Bishop?

### Setting up your python environment
Note that this is partially mentioned at the beginning of the lab.

You may not be familiar with virtual environments, but I suggest using one.  If you use anaconda as the lab suggests,
this can be done by running the command:
```
conda create --name ISLP
```
To activate it, run:
```
conda activate ISLP
```
In order to install the [ISLP](https://github.com/intro-stat-learning/ISLP) package to your virtual environment, you will need to install to install pip to it:
```
conda install pip
```
Now you can install the package with
```
pip install ISLP
```
