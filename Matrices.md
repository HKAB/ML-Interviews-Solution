1, 

Matrix is linear transformation

Linear transformation is the transformation that satisfy:
- T(x + y) = T(x) + T(y)
- T(cy) = cT(y)
        
Every linear transformation can be formulate as: T(v) = Av

2, 

Inverse of a matrix A is a matrix A^-1 that AA^(-1) = I. Not all matrix have an inverse, only square matrix with full rank have inverse. The inverse is unique.

3, 

The determinant of a matrix is a number that has spectial properties. If det(A) = 0 then the matrix is not invertible (singular).
    
4, 
    If we multiply a row by t, det(A_old) = t\*det(A_new)

5, 

trace(A) = sum_{eigenvalue} = 3 + 3 + 2 + -1

det(A) = multiply_{eigenvalue} = 3*3*2*(-1)
    
6, 

Because row 1 and row 3 is multiple of each other, we can conclude that the det is 0.

7, <later?>

8, 

i, The solution of the equation Ax = b can be writen in the form: x = x_p + x_h where x_p is a particular solution (a solution of Ax = b), x_h is the solution of the homogenerous system Ax = 0.
    
ii, The equation has unique solution when A has full rank (or b is in column space of A)
    
iii, When A has more columns than rows, the equation Ax = b has multiple solution. Consider x_h is the solution of Ax = 0, this equation must has solution that contains parameters, so there is infinite x_h, which lead to infinite x.
         
iv, <later?>