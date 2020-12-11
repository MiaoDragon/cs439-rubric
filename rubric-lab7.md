# Lab7 Rubric (Total Point 50)

## Part 1: Defining the Model and Feature Engineering (10)
### Task 1.1 Split the data into Y(tip) and X(all others) (4)

### Task 1.2: Feature Engineering (3)

### Task 1.2: Defining the Model (3)

## Part 2: Fitting the Model: Numeric Methods (5)
#### correctly use the loss function in the lambda expression with model to generate loss function (3)
#### correctly use scipy.optimize minimize to optimize (2)

## Part 3: Fitting the Model: Analytic Methods (15)
### Task 3.1: Least Squares Solution (6)
#### obtain X^TX theta = X^Ty (3)
#### obtain theta = (X^TX)^{-1}X^Ty (3)
### Task 3.2: Solving for Theta (6)
#### obtain X^TX and X^Ty (3)
#### obtain (X^TX)^{-1}X^Ty (3)
Notice that the analytical loss may not be the same as the template. It can be the following:
- if using **pinv** then the analytical solution should be close to the numerical solution, around 1.01
- if using **inv** then since the solver is not stable (can be dramatic difference in analytical loss), so we just ignore the analytical loss.

### Task 3.3: Weird Results? (3)
the student can show their reasoning for np.linalg.inv VS np.linalg.solve, or np.linalg.pinv VS np.linalg.solve. Anything mentioning the underlying numerical implementation would be awarded.

## Part 4 - Logistic Regression (20)
### task 4.1 (6)
#### get correct input X (3)
#### get correct output y (3)
### task 4.2 (4)
### task 4.3 logistic regression model (6)
#### construct logistic regression object (3)
#### fit the data (3)
### task 4.4 Predicting (2)
### task 4.5 reporting  (2)
