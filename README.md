# Stat 154: Modern Statistical Prediction and Machine Learning


- Instructor: Gaston Sanchez
- Lecture: 2 days p/week; 1.5 hours each day
- Midterm Exam: week 8
- Final: week 16
- Primary textbook:
    + CSL: Concepts of Statistical Learning (by Sanchez and Marzban, 2019)
- Secondary texts: 
    + ISL: An Introduction to Statistical Learning (by James et al, 2015)
    + ESL: The Elements of Statistical Learning (by Hastie et al, 2009)


-----

## 1. Introduction and Preamble for PCA

:speaker: __ABOUT__: We begin with some preliminary concepts and an overview of Statistical Learning methods. Then we discuss the concept of data as a set ob objects or individuals on which one or more variables have been measured. More specifically, we do this from a decisive geometric perspective.

:book: __READING__: 
- CSL Chapter 2: Introduction
- CSL Chapter 3: Geometric Duality

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
- CSL Chapter 4: Principal Component Analysis

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

:speaker: __ABOUT__: After PCA we shift gears to supervised learning methods that have to do with predicting a quantitative response. We begin with Linear Regression models which are the stepping stone for all supervised learning methods. We will study the general regression framework by paying attention to the algebraic and geometric aspects, while postponing the discussion of the learning elements for later (to be covered in Concepts of Learning Theory).

:book: __READING__: 
- CSL Chapter 5: Linear Reregssion
- CSL Chapter 6: Gradient Descent

:speech_balloon: __TOPICS__:
- __Introduction to Linear Regression__
    + Motivating an intuitive feeling for regression problems
    + The regression function: conditional expectation
    + Classic framework of Ordinary Least Squares (OLS)
- __Theoretical core of OLS and Optimization__
    + Geometries of Least Squares: individuals, variables, and parameters perspectives
    + Gradient descent algorithm
    + Linear regression from a probabilistic approach: Maximum Likelihood

