Path : [/Mathematics](<..\..\index.md>) [/Linear Algebra](<..\index.md>)
## Rank and Inverse of a Matrix

**Rank of a Matrix**

The rank of a matrix is a numerical measure of the dimensionality of the vector space spanned by its columns or rows. 

**Types of Rank:**

**1. Row Rank:**
- Number of linearly independent rows in a matrix.
- Row rank is equal to the dimension of the column space of the matrix.


**2. Column Rank:** 
- Number of linearly independent columns in a matrix.
- Column rank is equal to the dimension of the row space of the matrix.


**Rank can be determined by:**

- Row reduction
- Column reduction


**Inverse of a Matrix**

The inverse of a matrix is a matrix that "undoes" the action of the original matrix. 
- An invertible matrix has a multiplicative inverse.
- A matrix without an inverse is called a singular matrix.


**Conditions for the existence of a Matrix Inverse:**

- The matrix must be a square matrix.
- The matrix must be non-singular (determinant is not zero).


**Methods for finding the Inverse:**

- Gauss-Jordan elimination
- Adjoint method


**Relationship between Rank and Invertibility:**

- A square matrix is invertible if and only if its rank is equal to the order of the matrix. 
- A non-square matrix is never invertible.


**Applications of Rank and Inverse:**

**1. Solving Linear Equations:**
- The rank of the coefficient matrix determines the number of solutions to a system of linear equations.
- The inverse of the coefficient matrix can be used to solve the system.


**2. Finding Eigenvalues:**
- The rank of the matrix minus the identity matrix is related to the number of eigenvalues of the matrix.


**3. Singular Value Decomposition:**
- The rank of a matrix is equal to the number of non-zero singular values in its Singular Value Decomposition.


**Conclusion**

Rank and inverse are fundamental concepts in Linear Algebra that play a crucial role in various mathematical and engineering applications. Understanding these concepts is essential for solving linear equations, analyzing matrices, and performing various mathematical operations.
