Path : [/Mathematics](<..\..\index.md>) [/Numerical Methods](<..\index.md>)
## Fixed Point Iteration Method for Solving Nonlinear Algebraic Equations

**Introduction:**

Fixed point iteration is a numerical method used to find roots of nonlinear algebraic equations. 
$$f(x)=0$$

The method involves repeatedly applying a transformation that maps a point to itself, hoping to converge to a fixed point where the transformation leaves the point unchanged.


**Conditions for Convergence:**

* The function f(x) is continuous and differentiable in a neighborhood of the fixed point.
* The derivative of the function is less than one in magnitude in the neighborhood.


**Algorithm:**

1. Choose an initial guess x0.
2. Iterate using the following formula: 
$$x_{n+1} = g(x_n)$$ 
where g() is a function derived from f().
3. Repeat steps 1-2 until convergence is achieved.


**Methods for Finding g():**

* **Contraction Mapping:** g(x) = x - λf(x), λ < 1/2.
* **Projection Method:** g(x) = P(x), where P() is a contraction of the identity map.


**Applications:**

* Finding roots of polynomial equations.
* Finding equilibrium points in economic models.
* Solving boundary value problems.


**Example:**

Solve the equation x^2 - 2 = 0 using the fixed point iteration method.

**Solution:**

$$x_{n+1} = \frac{1}{2}(2 + x_n)$$

**Initial guess:** x0 = 1

**Iteration 1:** x1 = 1.5
**Iteration 2:** x2 = 1.3333
**Iteration 3:** x3 = 1.3055

**Converged Fixed Point:** x* = 1.3235

**Advantages:**

* Easy to implement.
* Widely applicable to various problems.
* Guaranteed convergence under certain conditions.


**Disadvantages:**

* May converge slowly for certain functions.
* May fail to converge if initial guess is far from the fixed point.
* Not suitable for highly non-linear equations.


**Conclusion:**

Fixed point iteration is a powerful method for solving nonlinear algebraic equations. Its simplicity and applicability make it a useful tool in various applications.
