# Lab5 Rubric (Total Point 50)
In general, no matter which method they are using, give them full points as long as result looks fine.

For the **image display**,
the image might seem wrong due to floating-point values. If the shown image seems off, then deduct point for image display.
if there appears a warning about clipping, but the shown image seems fine, then DON'T deduct point.

## Part 1: Pre-processing of an image (15)
### Task 1.1 Reading the image (6)
#### read image using matplotlib.image.imread (3)
#### show image using matplotlib.pyplot.imshow (3)
The shown image doesn't have to contain boundary values at axis limit (300 and 200 for y and x axes)

### Task 1.2: Splitting into RGB (9)
#### red image: correctly extract the R channel (1.5)
#### red image: make other channels 0 when plotting red image (1.5)
#### green image: correctly extract the G channel (1.5)
#### green image: make other channels 0 when plotting green image (1.5)
#### blue image: correctly extract the B channel (1.5)
#### blue image: make other channels 0 when plotting blue image (1.5)

## Part 2: Transforming images (15)
### Task 2.1: scale for first image A (2)
#### correctly scale image A by p (1)
#### show image (1)
since instrution is not clear, students are free to either create a function or just hard-code for this question.
If plot seems off, check the code.

### Task 2.2: scale for second image B (3)
#### correctly scale image B by some factor (1)
#### use 1-p as the scaling factor (1)
#### show image (1)
since instrution is not clear, students are free to either create a function or just hard-code for this question.
If plot seems off, check the code.

### Task 2.3: overlay image (5)
#### scale image A by p (1)
#### scale image B by 1-p (1)
#### sum of the two scaled image to obtain overlay image (2)
#### show image (1)
the image might seem wrong due to floating-point values. If the shown image seems off, then deduct point for this.
if there appears a warning about clipping, but the shown image seems fine, then DON'T deduct point.

### Task 2.4: Interactive panel (5)
#### function f can correctly overlay image given each alpha (3)
#### correctly create an interact panel, which shows overlayed image for each alpha after dragging. (2)
Some students might hardcode the image inside the function f due to some issues of interact package:
https://piazza.com/class/kenafi5hjxo4kq?cid=148
This is allowed.

## Part 3: Application of Singular Value Decomposition (15)
### Task 3.1: representation of matrix in 2D (1)
#### correctly extract RGB separately (1)

### Task 3.1: Finding Singular Values and Orthogonal matrices (2)
#### correctly use scipy.linalg.svd for each channel (2)

### Task 3.2: Finding a rank-1 approximation (4)
#### sort singular values (1)
#### extract u and v corresponding to the largest singular value (1)
#### matrix product using the extracted vectors and singular values to obtain low-rank approximation (1)
#### combine low-rank approximated RGB channels together into full image (0.5)
#### plot image (0.5)
Students are allowed to write a generic function to achieve rank-k approximation.

### Task 3.2: Finding a rank-2 approximation (4)
#### sort singular values (1)
#### extract u and v corresponding to the largest-2 singular value (1)
#### matrix product using the extracted vectors and singular values to obtain low-rank approximation (1)
#### combine low-rank approximated RGB channels together into full image (0.5)
#### plot image (0.5)

### Task 3.2: Finding a rank-k approximation (4)
#### sort singular values (1)
#### extract u and v corresponding to the largest-k singular value (1)
#### matrix product using the extracted vectors and singular values to obtain low-rank approximation (1)
#### combine low-rank approximated RGB channels together into full image (0.5)
#### plot image (0.5)

## Part 3 Open Ended Question (5)
Any reasonable answers will be accepted. Don't need to be long, and just need to list the possible applications.

## Lab Feedback (0)
