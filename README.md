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

## 1. Principal Components Analysis (PCA)

:speaker: __ABOUT__ We begin with Principal Components Analysis, one of the unsupervised learning topics of this course. Simply put, PCA allows us to study the systematic structure of a data set (of quantitative variables). Although PCA can be approached from multiple perspectives, we will approach it from a data visualization perspective, and a decisive geometric flavor.

:book: __READING__: 
- CSL Chapter 1: Introduction
- CSL Chapter 2: Geometric Duality

:speech_balloon: __TOPICS__
+ __Preamble for PCA__
	- The duality of the data matrix: rows (individuals) and columns (variables)
	- Common operations for individuals: the average individual, distance between individuals, multivariate dispersion, and inertia
	- Common operations for variables: variables as vectors, length of a vector, vector and scalar projections, angle between vectors, variance, covariance, correlation
+ __Fundamentals of PCA__
	- PCA from three perspectives: projected inertia, maximized variance, data decomposition
	- PCA solution with EVD of cross-products XTX and XXT

+ __Application of PCA (anatomy of PCA solution)__
	- How many components to retain? 
	- How can a component be interpreted?
	- What visualizations can be obtained, and how to read them?
	- Some practical considerations

+ __Digression on Matrix Decompositions__
	- Matrix decompositions: Eigenvalue Decomposition (EVD)
	- Singular Value Decomposition (SVD) and lower rank approximations
	- Relationship between EVD and SVD

