# Lab7 Rubric (Total Point 70+4)

## Question 1: Linear Regression (10)
### 1. Which of the following are suitable for a linear regression model? Select all that apply. (2)
#### Correct Answer: (a), (e)
#### 1 point for each answer.
#### if chosen wrong answer, then deduct 1 point, until 0 point

### 2.Given below is a plot of a data set (x,y) points.
#### (a) (1) sample solution: theta0=0, theta1=1
#### (b) (1) sample solution: theta0=0, theta1=1, theta2=0
#### (c) (1) sample solution: theta0=0, theta1=1, theta2=10
it’s approximately a sinusoid + linear function that passes through (0,0) and (5,-5) (we can approximately treat (5,-5) to be the lowest point of the sin). The linear function passes through (0,0) and (-10, -10).
The function is thus approximately

y = x + 10sinx

The given solution seems to have a y-axis that is not straight. So we should check students' answers by plotting and see if they fit individually.

### 3.
Since the hint mentions to look for a clear minima, most students have answered only in terms of this. None mentions the points in the rubric of differentiable, concave, convex, smooth. If they answered in terms of clear minima, give full points. 

if students showed why a and b are good then that's enough and we give full points.
#### (a) (1) 
##### Mention that the function is not smooth will be fine. The exact answer to whether it's "good" or not doesn't matter.
#### (b) (1) 
##### Mention smooth and convex/concave will be fine.
#### (c) (1) 
##### Mention that h(x)-y can be negative will be fine.
#### (d) (1) 
##### Mention that the function is unbounded, or not concave will be fine.

### 4. (1)
#### correct answer: (e)

## Question 2: Classification (10)
### 1. (5)
#### (a)  4  (1)
#### (b)  1  (1)
#### (c)  3  (1)
#### (d) 2/5  (2)

### 2. (5)
#### (a) (1)
##### Correct Answer: D.
##### reansoable explaination will be accepted. For instance, 3-1 split
#### (b) (1)
##### Correct Answer: B
#### (c) (1)
##### Correct Answer: C
#### (d) (2)
##### Correct Answer: D

## Question 3: Linear Algebra (10)
### 1. projection (1)
#### Acceptable answer: scalar projection, inner product of v and u
#### Acceptable answer: vector projection, inner product of v and u times u

### 2. sqrt(18)  (1)

### 3. not orthogonal since the inner product is nonzero (2)

### 4.
#### (a) the difference between the two rows are zero  (1)
##### Similar answers are accetable  
#### (b) the two random varaibles are orthogonal. Or not correlated. Or linearly independent.  (1)
notice that covariance being zero doesn't apply they are independent random variables, but only linearly independent.

### 5. plane  (2)
#### if draw something in 3d, or in other ways to answer something that is similar but not exactly plane, then give 1 pt.
### 6. <= 1/2 num of columns  (2)
#### if specify that rank will be reduced, but not mentioning the exact number, get 1 point

## Question 4 Regularization (10)
### 1. (2) 
#### Mention any of: penalize large coefficient, avoid overfitting, prefer small coefficients, add constraints/prior knowledge to parameters.
### 2.
#### (a) (2)
##### lambda sum theta^2  (need to include both lambda and the sum)
#### (b) (2)
##### make coefficients small (not sparse)
#### (c) (2)
##### mention any of: relax constraints on coeffcients value, large coefficients
#### (d) (2)
##### plot lambda vs. error and select the min one
##### Acceptable Answer: use validation set to select lambda

## Question 5. Unsupervised Learning (10)
### 1.(1)
#### Given correct answer: (b), (c), (e) (0.3pt for each one, 1pt if got all right)
treat (a) as a free point, and don’t deduct or give student’s points if they choose it
### 2.
#### (a) (1)
##### Random
#### (b) (1)
##### reasonable ones will be accepted: validation set, domain knowledge, iteratively increasing k until validation error dosen't decrease
#### (c) (1)
##### Acceptable answer: the overall error decreases
##### Acceptable answer: the training error decreases, but the testing error increases
#### (d) (1)
##### pull the center toward the outlier (0.5); 
##### remove outliers, or remove distance that is too large; assigning less weight to outliers (0.5)
#### (e) O((mk+m)t)  (1)
students can use 100 for t, hence O(100(mk+m))
##### 0.5pt if O(mkt), and 0.5pt if O(mt)
##### 0.5pt if solution is simplified
#### (f) Computing/Recomputing Centers  (1)

### 3.
#### (a) (1)
##### find centers iteratively to maximize center variation.
Also Accetable: find better centers
#### (b) (1)
##### Roughly same performance (1).
mentioning can have better center will also have full point.
#### (c) m(1+2+...+k-1)=O(mk(k-1)/2)  (1)

## Question 6. Deep Learning (10)
### 1.
#### (a) (1)
##### 3*4+4*2=20
#### (b) (1)
##### Mention any of: domain knowledge, validation test
##### a lot of students mentioned 2/3 of input+output size. Maybe they got this from some resources. We should give points as well.
### 2.
#### (a) (1.5)
##### theta1=1, theta2=1, theta0 can be [-2,-1)   (can be infinitely many correct ones, just check each one)
#### (b) (1.5)
##### theta1=1, theta2=1, theta0=-1              (can be infinitely many correct ones, just check each one)
#### (c) (1)
##### theta0=1, theta1=-2                        (can be infinitely many correct ones, just check each one)
Notice that students don't have to draw networks
### 3. (4)
#### (a) adding bias term to second layer 1--theta_6-->h(theta,x),
##### Possible Answer: theta0=20, theta1=-40, theta2=-40, theta3=-60, theta4=40, theta5=40, theta6=-20, theta7=40, theta8=40
Notice that if students only provide theta0, theta1 and theta2 would be fine as well. Since the problem didn't specify.
Also if students didn't draw the network it would be fine as well.

Some students might treat y1 and y2 as 0/1 outputs using sigmoid. If this way works we can give full point.

## Question 7. Recommendation System (10)
### 1. (2) 
#### example: recommending products, customized ads, email
### 2. (2)
#### example: incomplete information, changing user preference
### 3. (6)
#### ![equation](https://latex.codecogs.com/gif.latex?X_%7BAW%7D%3D3.5%2C%20X_%7BAZ%7D%3D3.5%2C%20X_%7BBX%7D%2C%20X_%7BBZ%7D%2C%20X_%7BCW%7D%3D3.75%2C%20X_%7BCY%7D%3D%2C%20X_%7BDW%7D%3D4.5)
#### ![equation](https://latex.codecogs.com/gif.latex?X_%7BBX%7D%3D%5Cbar%7Bx%7D_B&plus;%5Cfrac%7Bw_%7BBA%7D%28X_%7BAX%7D-%5Cbar%7Bx%7D_A%29&plus;w_%7BBD%7D%28X_%7BDX%7D-%5Cbar%7BX%7D_D%29%7D%7Bw_%7BBA%7D&plus;w_%7BBD%7D%7D%3D%5C%5C%20%5Cquad%5Cquad%5Cquad%5Cquad%20%5Cfrac%7B4.0&plus;3.5%7D%7B2%7D&plus;%5Cfrac%7B1.5%284.5-%284.5&plus;2%29/2%29&plus;1.5%283.5-%283.5&plus;4&plus;1%29/3%29%7D%7B1.5&plus;1.5%7D%3D0.95833)
#### Ignore the final result above, it should be X_BX = 4.7083
#### ![equation](https://latex.codecogs.com/gif.latex?X_%7BBZ%7D%3D%5Cbar%7Bx%7D_B&plus;X_%7BDZ%7D-%5Cbar%7Bx%7D_D%3D1.9167)
#### ![equation](https://latex.codecogs.com/gif.latex?X_%7BCY%7D%3D%5Cbar%7Bx%7D_C&plus;%5Cfrac%7Bw_%7BCA%7D%28X_%7BAY%7D-%5Cbar%7Bx%7D_A%29&plus;w_%7BCD%7D%28X_%7BDY%7D-%5Cbar%7Bx%7D_D%29%7D%7Bw_%7BCA%7D&plus;w_%7BCD%7D%7D%5C%5C%20%5Cquad%5Cquad%5Cquad%5Cquad%3D3.5&plus;%5Cfrac%7B0.5%282-3.25%29&plus;2.5%284-%5Cfrac%7B8.5%7D%7B3%7D%29%7D%7B3%7D%3D4.2639)
#### for the two missing parts, each one has 3 point.
#### if using the euqation provided, then 1.5 point for each part. (totally 3pt)

## Last Question 
### Nothing  0
### one very simple line of something 2
### more, a picture, etc. something interesting 4