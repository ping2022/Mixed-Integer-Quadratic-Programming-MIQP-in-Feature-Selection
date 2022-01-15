# Mixed Integer Quadratic Programming (MIQP) in Feature Selection
Comparison of Mixed Integer Quadratic Programming (MIQP) and LASSO in Feature Selection


# Introduction
As we know, one of the most common problems in predictive analytics is variable selection for regression. Because of computational difficulties, direct variable selection using optimization has long been dismissed by the statistics community. This computational issue was part of the motivation for the development of LASSO and ridge regression. However, in the recent past there have been tremendous advancements in optimization software such as Gurobi, specifically the ability to solve mixed integer quadratic programming (MIQP).

Therefore, we will pose the variable selection problem for regression as an MIQP, and compare it with LASSO. We will discuss the advantages and drawbacks of each method, and make recommendations on which method is better for which scenario.


# Approach
In our experimentation, there are 2 data sets that include x and y data. One data set is a training data set, and one is a test data set. We will first do 10-fold cross validation on the training set to pick k or λ. Then with the optimal values of k or λ we will fit βs using the entire training set. Then with those βs we will make a prediction of the y values on the test set, and compare our prediction of y to the true value of y in the test set.


# Blog
For a detailed explanation and report of this module, please refer to our blog: https://medium.com/@pingzhang0108/application-of-mixed-integer-quadratic-programming-miqp-in-feature-selection-for-regression-3985d2ab95a7


# Reference
[1] Resource: Bertsimas, D., & King, A. (2015). OR forum—An algorithmic approach to linear regression. Operations Research, 64(1), 2-16.
