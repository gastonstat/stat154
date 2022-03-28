# Stat 154: Modern Statistical Prediction and Machine Learning

- Description: This is an introductory course in statistical learning, with an emphasis on regression and classification methods (supervised learning), and a pinch of exploratory methods (unsupervised learning)
- Instructor: Gaston Sanchez
- Lecture: 2 days p/week; 1.5 hours each day
- Midterm Exam: week 8
- Final: week 16
- Primary textbook:
    + [CSL: Concepts of Statistical Learning](https://allmodelsarewrong.github.io/) (by Sanchez and Marzban, 2019)
- Secondary texts: 
    + ISL: An Introduction to Statistical Learning (by James et al, 2015)
    + ESL: The Elements of Statistical Learning (by Hastie et al, 2009)


-----

## 1. Introduction and Preamble for PCA

:speaker: __ABOUT__: We begin with some preliminary concepts and an overview of Statistical Learning methods. 
Then we discuss the concept of data as a set ob objects or individuals on which one or more variables have been 
measured. More specifically, we do this from a decisive geometric perspective.

:book: __READING__: 
- [CSL Chapter 2: Introduction](https://allmodelsarewrong.github.io/intro.html)
- [CSL Chapter 3: Geometric Duality](https://allmodelsarewrong.github.io/duality.html)

:speech_balloon: __TOPICS__:
+ __Preamble for PCA__
	- The duality of the data matrix: rows (individuals) and columns (variables)
	- Common operations for individuals: the average individual, distance between individuals, multivariate dispersion, and inertia
	- Common operations for variables: variables as vectors, length of a vector, vector and scalar projections, angle between vectors, variance, covariance, correlation


-----


## 2. Principal Components Analysis (PCA)

:speaker: __ABOUT__: Principal Components Analysis is one of the unsupervised learning topics of this course. 
Simply put, PCA allows us to study the systematic structure of a data set (of quantitative variables). 
Although PCA can be approached from multiple angles, we focus on its geometric perspective.

:book: __READING__: 
- [CSL Chapter 4: Principal Component Analysis](https://allmodelsarewrong.github.io/pca.html)

:speech_balloon: __TOPICS__:

+ __Fundamentals of PCA__
	- PCA from three perspectives: projected inertia, maximized variance, data decomposition
	- PCA solution with EVD of cross-products X'X and XX'
+ __Application of PCA (anatomy of PCA solution)__
	- How many components to retain? 
	- How can a component be interpreted?
	- What visualizations can be obtained, and how to read them?
	- Some practical considerations
+ __Digression on Matrix Decompositions__
	- Matrix decompositions: Eigenvalue Decomposition (EVD)
	- Singular Value Decomposition (SVD) and lower rank approximations
	- Relationship between EVD and SVD


-----

## 3. Linear Regression: Introduction

:speaker: __ABOUT__: After PCA we shift gears to supervised learning methods that have to do with predicting 
a quantitative response. We begin with Linear Regression models which are the stepping stone for all supervised 
learning methods. We will study the general regression framework by paying attention to the algebraic and 
geometric aspects, while postponing the discussion of the learning elements for later (to be covered in Concepts of Learning Theory).

:book: __READING__: 
- [CSL Chapter 5: Linear Reregssion](https://allmodelsarewrong.github.io/ols.html)
- [CSL Chapter 6: Gradient Descent](https://allmodelsarewrong.github.io/gradient.html)
- [CSL Chapter 7: Regression via Maximum Likelihood](https://allmodelsarewrong.github.io/olsml.html)

:speech_balloon: __TOPICS__:
- __Introduction to Linear Regression__
    + Motivating an intuitive feeling for regression problems
    + The regression function: conditional expectation
    + Classic framework of Ordinary Least Squares (OLS)
- __Theoretical core of OLS and Optimization__
    + Geometries of Least Squares: individuals, variables, and parameters perspectives
    + Gradient descent algorithm
    + Linear regression from a probabilistic approach: Maximum Likelihood


-----

## 4. Concepts of Learning Theory (part 1)

:speaker: __ABOUT__: In this part of the course we review the notion of Learning (from a supervised point of view) 
and other related concepts: What are the conceptual pieces of a learning problem? What do we mean by learning? 
How do we measure the learning ability of a machine/model? We will also talk about several aspects concerning 
Learning theory: model performance, bias-variance tradeoff, overfitting, validation, and model selection.

:book: __READING__: 
- [CSL Chapter 8: Theoretical Framework](https://allmodelsarewrong.github.io/learning.html)
- [CSL Chapter 9: MSE Estimator](https://allmodelsarewrong.github.io/mse.html)
- [CSL Chapter 10: Bias-Variance Tradeoff](https://allmodelsarewrong.github.io/biasvar.html)

:speech_balloon: __TOPICS__:
- __A framework for Supervised Learning__
    + Supervised Learning Diagram: anatomy of supervised learning problems
    + The meaning of Learning, and the need for Training and Test sets
    + Types of errors and their measures: In-sample and Out-of-sample errors
    + Noisy targets and conditional distributions
- __Bias-Variance trade-off__
    + Derivation of the Bias-Variance decomposition formula
    + Case study: data simulation to illustrate the bias-variance decomposition
    + Interpretation of the bias-variance trade-off


-----

## 5. Concepts of Learning Theory (part 2)

:speaker: __ABOUT__: In this part of the course we review the notion of Learning (from a supervised point of view) 
and other related concepts: What are the conceptual pieces of a learning problem? What do we mean by learning? 
How do we measure the learning ability of a machine/model? We will also talk about several aspects concerning 
Learning theory: model performance, bias-variance tradeoff, overfitting, validation, and model selection.

:book: __READING__: 
- [CSL Chapter 11: Overfitting](https://allmodelsarewrong.github.io/overfit.html)
- [CSL Chapter 12: Learning Phases](https://allmodelsarewrong.github.io/phases.html)
- [CSL Chapter 13: Resampling Approches](https://allmodelsarewrong.github.io/resampling.html)

:speech_balloon: __TOPICS__:
- __Overfitting__
    + What is overfitting? Why should we care about it? What causes overfitting?
    + Case study: data simulation to illustrate overfitting
- __Model Validation and Model Selection__
    + Validation: What is it? Why do we need it?
    + Validation holdout framework, and repeated validation, bootstrap validation
    + Three-way holdout frmework
    + Cross-Validation: k-fold CV, leave-one-out CV
    + Some general considerations


-----

## 6. Linear Regression: Regularization Methods (part 1)

:speaker: __ABOUT__: Having introduced the basic concepts of Learning Theory, we’ll expand our discussion of linear regression. The classic Least Squares solution for linear models is not always feasible or desirable. One main idea to get a better solution is by regularizing the regression coefficients. This can be done in a couple ways: 1) by transforming the predictors and reducing the dimensionality of the input space; or 2) by penalizing the criterion to be minimized via restricting the size of the regression coefficients.

:book: __READING__: 
- [CSL Chapter 14: Regularization Techniques](https://allmodelsarewrong.github.io/regular.html)
- [CSL Chapter 15: Principal Components Regression](https://allmodelsarewrong.github.io/pcr.html)
- [CSL Chapter 16: Partial Least Squares Regression](https://allmodelsarewrong.github.io/pls.html)

:speech_balloon: __TOPICS__:
- __Issues with Least Squares__
    + Issues with OLS and potential solutions (postponed from OLS regression)
    + Multicollinearity issues (postponed from OLS regression)
- __Regularization via Dimension Reduction methods__
    + Principal Components Regression (PCR)
    + Partial Least Squares Regression (PLSR)


-----

## 7. Linear Regression: Regularization Methods (part 2)

:speaker: __ABOUT__: Having introduced the basic concepts of Learning Theory, we’ll expand our discussion of linear regression. The classic Least Squares solution for linear models is not always feasible or desirable. One main idea to get a better solution is by regularizing the regression coefficients. This can be done in a couple ways: 1) by transforming the predictors and reducing the dimensionality of the input space; or 2) by penalizing the criterion to be minimized via restricting the size of the regression coefficients.

:book: __READING__: 
- [CSL Chapter 16: Ridge Regression](https://allmodelsarewrong.github.io/ridge.html)
- [CSL Chapter 17: Lasso Regression](https://allmodelsarewrong.github.io/lasso.html)

:speech_balloon: __TOPICS__:
- __Regularization via Penalized methods__
    + Ridge Regression (RR)
    + Other methods: lasso, elastic net, and cousins
    + Geometries of penalized parameters

