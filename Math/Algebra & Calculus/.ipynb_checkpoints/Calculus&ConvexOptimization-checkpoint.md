## 1, Differentiable functions

i, A function f(x) is differentiable at a if f'(a) exist.

ii, A function that doesn't have a derivative at a point: y = |x|

iii, A non-differentiable function that widely use in ML is ReLu: f(x) = max(x, 0). We can show that this function is not differentiable at x = 0 because the left side limit and right side limit is not equal (intuitively, the function is not smooth at x = 0).

[Reference](!https://sebastianraschka.com/faq/docs/relu-derivative.html)

## 2, Convexity

i, Convex function is a function that the graph has the property: No line segment of two point on the function is below the graph. Concave function property: No line segment of two point on the function is above the graph.

ii, The convex function is desirable in optimization problem because it has only one extreme point. 

iii, Intuition: Cross entropy loss is convex because the Hessian matrix has 0 as the lowest eigenvalue, so Hessian is postitive-define matrix -> convex. 

More: [Appendix](!https://jermwatt.github.io/machine_learning_refined/notes/6_Linear_twoclass_classification/6_2_Cross_entropy.html)

## 3, Logistic classifier

i, p(y = -1|x) = 1 - p(y = 1|x) = 1 - 1/(1 + e_{-z}) = e_{-z}/(e_{-z} + 1) = σ(-z)

ii, Without losing the generality, we assume the label is in {0, 1}.
L = -log(p(y_{i}|x)) = -log(σ(.)^{y_{i}}*(1 - σ(.)^{1 - y_{i}})) = -(y_{i}*σ(.) + (1 - y_{i})*(1 - σ(.))) which is the cross entropy function. The first derivative is: (y_{i} - σ(.))*x_{i}

iii, The result is the same from 2iii

## 4, First & Second Derivative

i, Second order derivative is use in the optimization step. For example consider: f(x + ϵ) = f(x) + ϵ*∇f(x) + 1/2!*ϵ^{T}*H*ϵ. H is the Hessian matrix which contain second order derivative information. To choose good ϵ, we solve the equation ∇f = 0, i.e ∇f(x) + H*ϵ = 0 -> ϵ = -H^{-1}*∇f(x).

ii, Second order derivative give us more information about the optimization process. It show how the derivative will change, so that we can adjust the learning rate 'adaptive' to the step. But calculate hessian take O(N^{2}) space and H must be invertible.

iii, Now we have some optimization algorithm approximate the H matrix to guild the optimization step. But calculate real H is really challenge for large neural network.

Reference: [D2l](!http://d2l.ai/chapter_optimization/gd.html)

## 5, Hessian matrix
To test for critical point, we calculate the eigenvalue of Hessian matrix.
If H is positive define matrix, then f attains local minimum at x.
If H is negative define matrix, then f attains local maximum at x.
If H has both negative and positive eigenvalue, then f attains saddle point at x.
Otherwise, the test is inconclusive.
Reference: [Wiki](!https://en.wikipedia.org/wiki/Hessian_matrix)

## 6, Jensen Inequality
Jensen inequality: E(f(X)) <= f(E(X)) (1), or in calculus form: \sum_{i}λ_{i}\*f(x_{i}) <= f(\sum_{i}λ_{i}x_{i}) (\sum_{i}λ_{i} = 1) (2).
Jensen's Inequality ensure the convex property of a function. Visually, the right is all the points of a line connect two point of the function while the left is all the points on the graph of the function. If the function is convex, all the point of the graph will always lie below the line connect any two point.

## 7, Chain rule
If g is differentiable at x and f is differentiable at g(x), then the composition function F = composition(f, g) have the derivative: F'(x) = F'(g(x))g'(x). Or in Leibniz form: dy/dx = dy/du\*du/dx

