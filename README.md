# Mixed-Integer-Quadratic-Programming-MIQP-in-Feature-Selection
Comparison of Mixed Integer Quadratic Programming (MIQP) and LASSO in Feature Selection

Linear regression is a supervised learning algorithm used to predict a quantitative response. One of the most common problems in predictive analytics is variable selection for regression. Because of computational difficulties, direct variable selection using optimization has long been dismissed by the statistics/analytics community. This computational issue was part of the motivation for the development of LASSO and ridge regression. However, in the recent past there have been tremendous advancements in optimization software such as Gurobi, specifically the ability to solve mixed integer quadratic programming (MIQP).

MIQP is the problem of optimizing a quadratic function over points in a polyhedral set where some of the components are restricted to be integral.

Therefore, we will pose the variable selection problem for regression as an MIQP, and compare it with LASSO. We will discuss the advantages and drawbacks of each method, and make recommendations on which method is better for which scenario.

In our experimentation, there are 2 data sets that include x and y data. One data set is a training data set, and one is a test data set. We will first do 10-fold cross validation on the training set to pick k or λ. Then with the optimal values of k or λ we will fit βs using the entire training set. Then with those βs we will make a prediction of the y values on the test set, and compare our prediction of y to the true value of y in the test set.

Please refer to our blog for a comprehensive analysis.
