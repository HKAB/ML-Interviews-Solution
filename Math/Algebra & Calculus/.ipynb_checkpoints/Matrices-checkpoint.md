## 1, Linear Transformation & Matrix
Matrix is linear transformation

Linear transformation is the transformation that satisfy:
- T(x + y) = T(x) + T(y)
- T(cy) = cT(y)
        
Every linear transformation can be formulate as: T(v) = Av

## 2, Inverse of a matrix
Inverse of a matrix A is a matrix A^-1 that AA^(-1) = I. Not all matrix have an inverse, only square matrix with full rank have inverse. The inverse is unique.

## 3, Determinant of a matrix 
The determinant of a matrix is a number that has spectial properties. If det(A) = 0 then the matrix is not invertible (singular).
    
## 4, Property of determinant
If we multiply a row by t, det(A_old) = t\*det(A_new)

## 5, Trace & determinant of matrix
trace(A) = sum_{eigenvalue} = 3 + 3 + 2 + -1

det(A) = multiply_{eigenvalue} = 3*3*2*(-1)
    
## 6, Calculate determinant
Because row 1 and row 3 is multiple of each other, we can conclude that the det is 0.

## 7, Covariance matrix and Gram matrix

## 8, Solution of Ax = b
i, The solution of the equation Ax = b can be writen in the form: x = x_p + x_h where x_p is a particular solution (a solution of Ax = b), x_h is the solution of the homogenerous system Ax = 0.
    
ii, The equation has unique solution when A has full rank (or b is in column space of A)
    
iii, When A has more columns than rows, the equation Ax = b has multiple solution. Consider x_h is the solution of Ax = 0, this equation must has solution that contains parameters, so there is infinite x_h, which lead to infinite x.
         
iv, <later?>

## 9, Derivative, Gradient & Jacobian
i, The derivative of a function represent the rate change of a function.
ii, The derivative is a function measure the rate change of a function at a point. A gradient of a function (f: R^{n} -> R) is a vector represent the direction which make the function f reduce the most. A Jacobian matrix of a function (f: R^{m} -> R^{n}) is a matrix of partial derivative of size m x n. 

## 10, Jacobian
m x (n x d) (i guess?)