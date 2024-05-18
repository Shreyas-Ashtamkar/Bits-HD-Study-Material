Path : [/Mathematics](../../index.md) [/Linear Algebra](../index.md)
## Range and Kernel of a Linear Transformation

**Linear Transformation:**

A linear transformation is a function that satisfies two key properties:

1. **Homogeneity:** T(c * u) = c * T(u) for any scalar c and vector u.
2. **Additivity:** T(u + v) = T(u) + T(v) for any vectors u and v.


**Range:**

* The range of a linear transformation T is the set of all vectors that can be produced by applying T to any vector from the domain.
* It is denoted by rng(T) or im(T).
* The range represents the span of the images of the basis vectors.


**Kernel:**

* The kernel of a linear transformation T is the set of all vectors that are transformed to the zero vector.
* It is denoted by ker(T).
* The kernel represents the subspace where the transformation "annihilates" vectors.


**Relationship between Range and Kernel:**

The dimension of the range plus the dimension of the kernel equals the dimension of the domain. This is known as the **Rank-Nullity Theorem**.

$$dim(domain) = dim(range) + dim(kernel)$$

**Examples:**

**1) Identity Transformation:**

* Identity transformation maps a vector to itself.
* Range = span of the domain
* Kernel = {0}


**2) Rotation in Euclidean space:**

* Counterclockwise rotation by 90 degrees.
* Range = Span of the original space, excluding the z-axis.
* Kernel = Span of the z-axis.


**3) Scaling in Euclidean space:**

* Scaling by a factor of 2.
* Range = Span of the original space.
* Kernel = {0}


**Properties of Range and Kernel:**

* The range is a subspace of the codomain.
* The kernel is a subspace of the domain.
* The range and kernel are complementary subspaces to the domain and codomain respectively.


**Applications:**

* **Finding solutions to linear equations:** The kernel represents the space of solutions.
* **Determining the rank of a matrix:** The rank is equal to the dimension of the range.
* **Analyzing data:** The range can be used to describe the spread of data, while the kernel can be used to identify patterns.


**Conclusion:**

The range and kernel are fundamental concepts in Linear Algebra, playing crucial roles in understanding the behavior of linear transformations. Their properties have numerous applications in diverse fields, including mathematics, engineering, and physics.
