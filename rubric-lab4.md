# Lab4 Rubric (Total Point 50)
In general, no matter which method they are using, give them full points as long as result looks fine.

## Part 1: Scaling (21)
### 2.1 Question 1.1 (3)
#### select the correct column for Female Adult Literacy (1)
#### select the correct column for Gross National Income Per Capita (1)
#### create a new dataframe containing the two columns (order DOSEN'T matter) (1)
#### drop NaN rows (optional)

### 2.2 Question 1.2 (3)
order of plots do not matter. They can be stacked vertically or horizontally.
#### plot for Female Adult Literacy (1.5)
order of country names in the plot dosen't matter, as long as the values seem correct would be fine.
No need to strictly match the plot in the template.
#### plot for Gross National Income Per Capita (1.5)
order of country names in the plot dosen't matter, as long as the values seem correct would be fine.
No need to strictly match the plot in the template.


### 2.3 Question 1.3 (2)
reasonable answers that cover these:
1. mention the limitation of histogram (works with numerical data in both axis), and the country name is nominal data.
2. countplot is NOT the right tool for the job because we're currently analyzing quantitative data. Countplot is a vizualization tool traditionally used for categorical data
3. countplot is used for categorical data.but literacy rates and income per capita are numerical variables
4. too many specific individual values for the literacy rates and gross national income rates. in both graphs most of the values just have a single count.
5. count for gross income per capita doesn't make sense
6. In our data the index of each row is based on the country. So naturally we would want to understand the income and literacy rate referring to each country rather than how many countries match a literacy rate or income per capita
7. too many datapoints in x-axis. (make sense because if the datapoints are fewer, then it's easier to tell from countplot)

### 2.4 Question 1.4 (3)
order of plots do not matter. They can be stacked vertically or horizontally.
#### if they didn't specify y=df.index, which thus shows a single bar in each plot, then we deduct 1 point in total.
#### plot for Female Adult Literacy (1.5)
order of country names in the plot dosen't matter, as long as the values seem correct would be fine.
No need to strictly match the plot in the template.
#### plot for Gross National Income Per Capita (1.5)
order of country names in the plot dosen't matter, as long as the values seem correct would be fine.
No need to strictly match the plot in the template.

### 2.5 Question 1.5 (3)
order of plots do not matter. They can be stacked vertically or horizontally.
#### plot for Female Adult Literacy (1.5)
No need to strictly match the plot in the template, as long as the values seem correct.
#### plot for Gross National Income Per Capita (1.5)
No need to strictly match the plot in the template, as long as the values seem correct.

### 2.6 Question 1.6 (2)
order of plots do not matter. They can be stacked vertically or horizontally.
#### plot for Female Adult Literacy (1)
No need to strictly match the plot in the template, as long as the values seem correct.
#### plot for Gross National Income Per Capita (1)
No need to strictly match the plot in the template, as long as the values seem correct.

### 2.7 Question 1.7 (2)
order of plots do not matter. They can be stacked vertically or horizontally.
#### plot for Female Adult Literacy (1)
No need to strictly match the plot in the template, as long as the values seem correct.
#### plot for Gross National Income Per Capita (1)
No need to strictly match the plot in the template, as long as the values seem correct.

### 2.8 Question 1.8 (3)
#### plot might be different from the template because students didn't remove the NA before. This is fine as long as code is correct. We should still give full points if correct.
#### logarithmic transformation of data (2)
check code if plot is not correct for this part.
#### plot for Gross National Income Per Capita (1)
No need to strictly match the plot in the template, as long as the values seem correct.
If the plot does not seem correct, check if logarithmic is correct. If the logarithmic transform
is wrong, but the plot is consistent with the wrongly transformed value, then give points for plotting

## Part 2: Kernel Density Estimation (24)
#### If students didn't use correct datapoint, we can correct it for them ([2,4,9]). If result is correct, they still get full point.

### 4.1 Question 2.1
#### function implementation (2)
can directly check correctness by the plot
### 4.2 Question 2.2 (3)
students can use for loop, numpy array, or just manually copy code for each plotting. As long as the
plot values match the one in template would be good.
Just need to check the plot values. The axis limit and other plot details don't need to be strict.
#### use gaussian kernel separately for each datapoint (2)
can check code if the plot seems wrong to make sure students actually used gaussian kernel for each datapoint
#### plot distributions in the same axis (1)

### 4.3 Question 2.3 (4)
#### sum of all kernels (2)
#### normalize after sum (check value range for this part) (1)
#### plot matches the one in the template (1)
don't have to strictly match, just check if value seems reasonable.

### 4.4 Question 2.4 (1)
#### plot as before in Question 1.8 (check template) (1)

### 4.5 Question 2.5 (6)
#### use world bank data and logarithmic transform of the datapoint (2)
#### sum of all kernels (2)
#### normalize after sum (check value range for this part) (1)
#### tuned alpha so that plot matches the one in the template (1)
don't need to be strict, as long as shape looks similar will be fine

### 4.6 Question 2.6 (6)
#### used the kernel argument passed to compute KDE (1)
#### sum of all kernels (2)
#### normalize after sum (1)
#### other correctness (2)
If the plot doesn't show density, it might be due to NaN values. In this case, we can help them filter out nan using np.isnan.
can check template for correctness

### 4.7 Question 2.7 (2) Free Points
#### the font size is too small. Let's just give them free points for this question.
#### compare and contrast Gaussian and Boxcar kernels. Any reasonable answers will get full mark.

## Lab Feedback (5)
