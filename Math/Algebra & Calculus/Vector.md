# Vectors

Resource for quick refresh: [Elementary Linear Algebra](http://www.astronomia.edu.uy/progs/algebra/Larson%20-%20Edwards%20y%20Falvo%20Elementary%20Linear%20Algebra.pdf), [Calculus early transcendentals](https://www.amazon.com/Calculus-Early-Transcendentals-James-Stewart/dp/1285741552)

### 1. Dot product

The dot product between u and v is

\begin{align} u\cdot v=\| u\| \ \| v\| \ \cos( \theta ) \end{align}

The dot product give us a scalar. A quick look can gave us insight that dot product has something to do with the angle between them. || u || * cos(theta) represent the magnitude of the vector u when projected to v. So the dot product is the times of two magnitude of two vector pointing at the same direction (direction of v).

Additional material: [Wolframalpha](https://mathworld.wolfram.com/DotProduct.html)

The dot product is maximum when cos(theta) = 1. So the v is the unit vector of u:

\begin{align} v=\ \frac{u}{\| u\| } \end{align}

### 2. Outer product

Outer product of [3 2 1] and [-1 0 1] is [[-3 0 3], [-2 0 2], [-1 0 1]]

Purpose: Matrix factorization? (I haven't learned about this)

### 3. Linear Independence

Two vector a, b is said to be linearly independence if one vector can't be construct by other multiply by a scalar. Or mathematically c1\*a + c2\*b = 0 have trivial solution c1 = 0, c2 = 0
