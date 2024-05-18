Path : [/Mathematics](../../index.md) [/Complex Variables](../index.md)
## Cauchy's Integral Formula

**Cauchy's integral formula** is a fundamental theorem in complex analysis that relates the values of a function at a point to its behavior along a closed contour surrounding that point. 

**Formula:**

$$f(a)=\frac{1}{2i\pi}\oint_\gamma \frac{f(z)}{(z-a) }dz$$

**Where:**

- \(f(z)\) is an analytic function on an open set containing the closed contour \(\gamma\).
- \(a\) is a point interior to \(\gamma\).


**Applications:**

- Finding analytic continuation of functions
- Studying singularities of functions 
- Evaluating complex integrals by reducing them to contour integrals 


**Conditions for applicability:**

- The function \(f(z)\) is analytic inside and on the closed contour \(\gamma\).
- The contour should enclose only one singularity.


**Procedure to apply the formula:**

1. Choose a closed contour \(\gamma\) which encloses the singularity \(a\).
2. Parameterize the contour \(\gamma\).
3. Evaluate the complex integral along the contour using the parameterization.
4. Apply Cauchy's integral formula to obtain the desired result.


**Examples:**

**Finding the derivative of a function:**

$$f'(a)=\frac{1}{2i\pi}\oint_\gamma \frac{f(z)}{(z-a)^2}dz$$

**Evaluating a complex integral:**

$$\int_\gamma \frac{\sin(z)}{(z-i)}dz=2i\sin(i)$$

**Properties:**

- The integral is independent of the shape of the contour as long as it encloses the singularity.
- If the contour is large and far away from the singularity, the integral tends to zero.


**Cauchy's integral formula has numerous applications in various fields, including:**

- Engineering: Analyzing electrical circuits
- Physics: Studying wave propagation
- Applied mathematics: Solving partial differential equations


**Note:** 

- The complex integral is typically evaluated using residue theory.
- Cauchy's integral formula is a fundamental tool for understanding and manipulating analytic functions in complex analysis.
