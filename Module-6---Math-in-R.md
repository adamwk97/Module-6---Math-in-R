Math in R Part 2
================

Working with math in R and matrices.

``` r
A=matrix(c(2,0,1,3), ncol=2)
B=matrix(c(5,2,4,-1), ncol=2)
sumAB = A+B
sumAB
```

         [,1] [,2]
    [1,]    7    5
    [2,]    2    2

``` r
diffAB = A-B
diffAB
```

         [,1] [,2]
    [1,]   -3   -3
    [2,]   -2    4

A+B creates a 2x2 matrix with values 7, 2, 5, 2, and A-B creates a 2x2 matrix with values -3, -2, -3, 4

``` r
diag = diag(c(4,1,2,3), 4, 4)
diag
```

         [,1] [,2] [,3] [,4]
    [1,]    4    0    0    0
    [2,]    0    1    0    0
    [3,]    0    0    2    0
    [4,]    0    0    0    3

``` r
m = diag(3, 5, 5)
m[1,] = 1
m[,1] = 2
m[1,1] = 3
m
```

         [,1] [,2] [,3] [,4] [,5]
    [1,]    3    1    1    1    1
    [2,]    2    3    0    0    0
    [3,]    2    0    3    0    0
    [4,]    2    0    0    3    0
    [5,]    2    0    0    0    3

Using the 'diag' function, we can first create a matrix with the diagonal values set to 3, and then append the other values accordingly.
