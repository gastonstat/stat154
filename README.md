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
Then we discuss the concept of data as a set of objects or individuals on which one or more variables have been 
measured. More specifically, we do this from a decisive geometric perspective.

:book: __READING__: 
- [CSL: Introduction](https://allmodelsarewrong.github.io/intro.html)
- [CSL: Geometric Duality](https://allmodelsarewrong.github.io/duality.html)

:speech_balloon: __TOPICS__:
+ __Preamble for PCA__
	- The duality of the data matrix: rows (individuals) and columns (variables)
	- Common operations for individuals: the average individual, distance between individuals, multivariate dispersion, and inertia
	- Common operations for variables: variables as vectors, length of a vector, vector and scalar projections, angle between vectors, mean, variance, covariance, and correlation


-----


## 2. Principal Components Analysis (PCA)

:speaker: __ABOUT__: Principal Components Analysis is one of the unsupervised learning topics of this course. 
Simply put, PCA allows us to study the systematic structure of a data set (of quantitative variables). 
Although PCA can be approached from multiple angles, we focus on its geometric perspective.

:book: __READING__: 
- [CSL: Principal Component Analysis](https://allmodelsarewrong.github.io/pca.html)

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
- [CSL: Linear Reregssion](https://allmodelsarewrong.github.io/ols.html)
- [CSL: Gradient Descent](https://allmodelsarewrong.github.io/gradient.html)
- [CSL: Regression via Maximum Likelihood](https://allmodelsarewrong.github.io/olsml.html)

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
- [CSL: Theoretical Framework](https://allmodelsarewrong.github.io/learning.html)
- [CSL: MSE Estimator](https://allmodelsarewrong.github.io/mse.html)
- [CSL: Bias-Variance Tradeoff](https://allmodelsarewrong.github.io/biasvar.html)

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
- [CSL: Overfitting](https://allmodelsarewrong.github.io/overfit.html)
- [CSL: Learning Phases](https://allmodelsarewrong.github.io/phases.html)
- [CSL: Resampling Approches](https://allmodelsarewrong.github.io/resampling.html)

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
- [CSL: Regularization Techniques](https://allmodelsarewrong.github.io/regular.html)
- [CSL: Principal Components Regression](https://allmodelsarewrong.github.io/pcr.html)
- [CSL: Partial Least Squares Regression](https://allmodelsarewrong.github.io/pls.html)

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
- [CSL: Ridge Regression](https://allmodelsarewrong.github.io/ridge.html)
- [CSL: Lasso Regression](https://allmodelsarewrong.github.io/lasso.html)

:speech_balloon: __TOPICS__:
- __Regularization via Penalized methods__
    + Ridge Regression (RR)
    + Other methods: lasso, elastic net, and cousins
    + Geometries of penalized parameters


-----

## 8. Regression: Moving Beyond Linearity (time permitting)

:speaker: __ABOUT__: Linear models can be quite useful but they have some limitations that force us to move beyond linearity. The main idea in this section is to relax the linearity assumption while still trying to obtain interpretable models. We’ll learn about various approaches that allow us to augment/replace the input variables with an array of transformations such as polynomial regression, step functions, splines, local regression, RBF, etc.

:book: __READING__: 
- [CSL: Beyond Linear Regression](https://allmodelsarewrong.github.io/linear-extensions.html)
- [CSL: Basis Expansion](https://allmodelsarewrong.github.io/basis.html)
- [CSL: Nonparametric Regression](https://allmodelsarewrong.github.io/nonparametric.html)
- [CSL: Nearest Neighbors Estimates](https://allmodelsarewrong.github.io/knn.html)
- [CSL: Kernel Smoothers](https://allmodelsarewrong.github.io/kernel-smoothers.html)

:speech_balloon: __TOPICS__:
- __Limitation of linear models, and notion of linearity__
    + Some nonlinear approaches
    + Polynomial regression
    + Stepwise regression
    + Basis functions (basis-expansion)
    + Splines
    + Local regression
    + Radial Basis Functions


-----

## 9. Introduction to Classification

:speaker: __ABOUT__: The other major type of supervised learning problems covered in this course has to do with classification methods: predicting a qualitative response. We begin with Logistic Regression which provides a nice bridge between linear regression and classification ideas.

:book: __READING__: 
- [CSL: Classification](https://allmodelsarewrong.github.io/classif.html)
- [CSL: Basis Expansion](https://allmodelsarewrong.github.io/logistic.html)

:speech_balloon: __TOPICS__:
- __Introduction to Classification__
    + The classification problem
    + Limitations of the classic regression model
    + Motivation for logistic transformation
- __Logistic Regression__
    + Model
    + Error measure
    + Algorithm(s)


-----

## 10. Discriminant Analysis (part 1)

:speaker: __ABOUT__: An important kind of classification methods belong to a general framework known as Discriminant Analysis (DA). We start reviewing certain notions and formulas to measure total variation (or dispersion) in terms of a) variation within classes and b) variation between classes. Then we discuss Ronald Fisher's geometric approach commonly known as Canonical Discriminant Analysis. This method can be considered to be a classification with an unsupervised touch. 

:book: __READING__: 
- [CSL: Preamble for Discriminant Analysis](https://allmodelsarewrong.github.io/discrim.html)
- [CSL: Canonical Discriminant Analysis](https://allmodelsarewrong.github.io/cda.html)

:speech_balloon: __TOPICS__:
- __Preamble for Discriminant Analysis__
    + Total variation decomposition
    + Variation within classes
    + Variation between classes
- __Canonical Discriminant Analysis (CDA)__
    + CDA's semi-supervised approach
    + CDA's supervised approach
    + Limitations of CDA classifiers


-----

## 11. Discriminant Analysis (part 2) and Performance in Classification Methods

:speaker: __ABOUT__: We continue the discussion of Discriminant Analysis (DA) with the so-called generative classification methods: Linear DA, Quadratic DA, and Naives Bayes. Then we move onto model performance with classification methods. Similar to what we did for regression models, we will discuss how to assess model performance in a classification setting. We will also talk about concepts like: confusion matrices, sensitivity and specificity, true positives and false positives, as well as Receiver Operating Characteristic (ROC) curves. 

:book: __READING__: 
- [CSL: Discriminant Analysis](https://allmodelsarewrong.github.io/discanalysis.html)
- [CSL: Perfomance of Classifiers](https://allmodelsarewrong.github.io/classperformance.html)

:speech_balloon: __TOPICS__:
- __Discriminant Analysis__
    + Probabilistic Discriminant Analysis
    + Linear Discriminant Analysis (LDA)
    + Quadratic Discriminant Analysis (QDA)
    + Naive Bayes
- __Performance of Classifiers__
    + Measures of Classification Error
    + Confusion Matrices
    + Decision Rules
    + ROC Curves


-----

## 12. Clustering Methods

:speaker: __ABOUT__: Simply put, Clustering has to do with finding groups in data. This is the second unsupervised topic of the course, covering partition methods as well as hierarchical agglomerative techniques.

:book: __READING__: 
- [CSL: Clustering](https://allmodelsarewrong.github.io/clustering.html)
- [CSL: K-Means](https://allmodelsarewrong.github.io/kmeans.html)
- [CSL: Hierarchical Clustering](https://allmodelsarewrong.github.io/hclus.html)

:speech_balloon: __TOPICS__:
- __Clustering__
    + About clustering
    + Dispersion measures
    + Complesity in clustering
- __Direct Partitioning Methods__
    + Partitioning methods
    + K-Means
- __Hierarchical Clustering__
    + Distances and Dissimilarities
    + Single linkage
    + Complete linkage
    + Average linkage
    + Centroid linkade
    + Dendrograms


-----

## 13. Tree-Based Methods (part 1)

:speaker: __ABOUT__: We introduce decision trees, which are one the most visually atractive and intuitive supervised learning methods. In particular, we will focus our discussion around one kind of trees, the CART-style binary decision trees from the methodology developed in the early 1980s by Leo Breiman, Jerome Friedman, Charles Stone, and Richard Olshen.

:book: __READING__: 
- [CSL: Trees](https://allmodelsarewrong.github.io/trees.html)
- [CSL: Binary Splits and Impurity](https://allmodelsarewrong.github.io/tree-impurities.html)

:speech_balloon: __TOPICS__:
- __Introduction to Trees__
    + Terminology
    + Tree diagrams
- __Binary splits and impurity__
    + Binary partitions
    + Measures of impurity: Entropy
    + Measures of impurity: Gini impurity
    + Measures of impurity: Variance-based


-----

## 14. Tree-Based Methods (part 2)

:speaker: __ABOUT__: We introduce decision trees, which are one of the most visually atractive and intuitive supervised learning methods. In particular, we will focus our discussion around one kind of trees, the CART-style binary decision trees from the methodology developed in the early 1980s by Leo Breiman, Jerome Friedman, Charles Stone, and Richard Olshen.

:book: __READING__: 
- [CSL: Splitting Nodes](https://allmodelsarewrong.github.io/tree-splits.html)
- [CSL: Building Binary Trees](https://allmodelsarewrong.github.io/tree-basics.html)

:speech_balloon: __TOPICS__:
- __Splitting Nodes__
    + Entropy-based splits
    + Gini-impurity based splits
    + Looking for the best split
- __Building Binary Trees__
    + Node-splitting stopping criteria
    + Pruning a tree
    + Pros and cons of trees


-----

## 15. Ensemble Methods and Aggregation

:speaker: __ABOUT__: We finish the course with so-called Ensemble methods (i.e. aggregating individual learners) such as baging, boosting, and random forests.

:book: __READING__: 
- [CSL: Bagging](https://allmodelsarewrong.github.io/bagging.html)
- [CSL: Random Forests](https://allmodelsarewrong.github.io/forest.html)

:speech_balloon: __TOPICS__:
- __Bagging: bootstraop aggregating__
    + Idea of bagging
    + Advantages of bagging
- __Random Forests__
    + Idea of random forest
    + Advantages of random forest

