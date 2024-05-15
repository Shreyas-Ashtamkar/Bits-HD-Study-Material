Path : [/Mathematics](<..\..\index.md>) [/Numerical Methods](<..\index.md>)
## Method of False Position

**Solution of Nonlinear Algebraic Equations**

The method of false position (MFP) is a root-finding algorithm used to locate the roots of non-linear algebraic equations. It stands out as a simple and direct numerical technique for finding roots.

**Principle of Operation**

The method employs the concept of bracketing and bisection to narrow down the interval containing the root. It follows a two-step process:

**1. Braketing:**
- Choose two initial guesses, x1 and x2, such that f(x1) and f(x2) have opposite signs. 
- This creates an initial interval [x1, x2] containing the root.

**2. Interpolation:**
- Draw a straight line between (x1, f(x1)) and (x2, f(x2)).
- The point where this line intersects the x-axis is the predicted root.
- The new interval is formed by taking the point closest to the root and the point where the function changes sign.

**Algorithm**

```
1. Input: f(x), x1, x2, tolerance
2. While |x2 - x1| > tolerance:
    - Calculate the midpoint, x = (x1 + x2) / 2.
    - If f(x1) * f(x) < 0:
        - Update x2 = x.
    - Otherwise:
        - Update x1 = x.
3. Return x as the approximate root.
```

**Examples**

**Example 1:** Find the root of the equation x^2 - 2x - 5 = 0.

- Choose x1 = 2 and x2 = 3.
- The bracket is [2, 3].
- The root is approximately 2.309.

**Example 2:** Solve the equation x^3 - 2x - 5 = 0.

- Choose x1 = 1 and x2 = 2.
- The bracket is [1, 2].
- The root is approximately 1.84.

**Advantages**

- Simple and easy to implement.
- Only function evaluations are required.
- Guaranteed to converge when the function is continuous and changes sign.

**Disadvantages**

- Not suitable for highly oscillatory functions.
- Accuracy can be slow for certain problems.
- Can be unstable for large initial intervals.

**Applications**

- Finding roots of polynomials.
- Numerical optimization problems.
- Finding intersection points of curves.
