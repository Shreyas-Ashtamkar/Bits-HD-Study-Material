Path : [/Mathematics](../../index.md) [/Differential Equations](../index.md)
## Higher Order Linear Differential Equations with Constant Coefficient

**Definition:**

A higher order linear differential equation (HODLE) with constant coefficients is an equation containing derivatives of a function of a single independent variable and its coefficients are constants. 


**General form:**

$$a_n \frac{d^n y}{dx^n} + a_{n-1}\frac{d^{n-1} y}{dx^{n-1}} + ... + a_1\frac{dy}{dx} + a_0y = f(x)$$

where:
* \(a_i\) are constant coefficients
* \(y\) is the unknown function
* \(f(x)\) is a known function


**Solving HODLEs:**

Solving HODLEs with constant coefficients generally requires applying specific techniques such as:

**1. Characteristic equation method:**
- Extract the coefficients of the highest derivative and the constant term.
- Solve the characteristic equation to obtain the auxiliary equation.
- Use the solution of the auxiliary equation to form the general solution of the HODLE.


**2. Variation of parameters:**
- Assume a solution of the form \(y=e^{\lambda x}\) and substitute it into the equation.
- Solve for \(\lambda\) to obtain a set of linear equations.
- Solve the linear equations to obtain the coefficients of the power series solution.


**3. Power series solution:**
- Assume a power series solution of the form \(y = \sum_{n=0}^\infty a_nx^n\).
- Substitute the power series into the equation and collect terms.
- Equating coefficients of like powers of \(x\) gives a set of recursion relations for the coefficients.


**Applications:**

HODLEs with constant coefficients have numerous applications in various fields, including:

* **Engineering:** modeling vibrations, electrical circuits, and fluid dynamics.
* **Physics:** describing wave propagation, harmonic oscillators, and heat flow.
* **Finance:** modeling interest rates and financial derivatives.


**Examples:**

**1) Solve the following HODLE:**
$$y''-4y'+3y=x$$

**Solution:** Using the characteristic equation method, we obtain the general solution: $$y=c_1 e^{3x} + c_2 e^{-x}$$

**2) Find the solution to the following boundary value problem:**
$$y''+4y=0, \quad y(0)=1, \quad y(\pi/2)=0$$

**Solution:** Using separation of variables, we obtain the solution: $$y= \sin(2x)$$


**Conclusion:**

HODLEs with constant coefficients play a significant role in various scientific and engineering applications. Understanding their solution techniques and applications is essential for solving a wide range of mathematical problems that arise in diverse fields.
