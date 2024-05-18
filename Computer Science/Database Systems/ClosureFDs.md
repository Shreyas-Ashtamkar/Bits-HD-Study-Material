Path : [/Computer Science](../../index.md) [/Database Systems](../index.md)
## Closure of a Set of FDs

**Definition:**

The closure of a set of functional dependencies (FDs) is a set of additional FDs derived from the given set. It ensures that all the implications of the initial FDs are also captured. In database systems, closure helps to determine the candidate keys of a relation.

**Closure Construction:**

Given a set of FDs, we can obtain their closure by applying the following closure rules repeatedly until no new FDs can be derived:

**1. Transitivity:**
- If A->B and B->C, then A->C.

**2. Union:**
- If A->B and A->C, then A->BC.

**3. Functional Dependency:** 
- If A->B and not exist another attribute set X such that X->B, then AB->B.


**Example:**

Consider the relation schema:

```
Student(Name, Email, Course, Year)
```

And the following FDs:

```
Name -> Email
Course -> Year
```

The closure of this set of FDs is:

```
Name -> Email
Course -> Year
Name -> Year
```

**Key Properties of Closure:**

- Closure is a closure operation.
- The closure of a set of FDs is a set of FDs.
- The closure of a set of FDs is the smallest set of FDs that contains the given set.

**Applications of Closure:**

- **Identifying candidate keys:** 
    - A candidate key is a set of attributes that uniquely determines every tuple in a relation.
    - The closure of a set of FDs can help identify candidate keys by ensuring that all tuple pairs that are related by some FD are also related by the candidate key.
- **Data integrity constraints:**
    - FDs are important data integrity constraints as they guarantee that changes to one attribute can be automatically reflected in other attributes.
    - The closure of a set of FDs ensures that these constraints are preserved in the database.


**Closure and Normalization:**

- **Normal forms:** A relation is in normal form (NF) if it satisfies certain criteria based on its FDs.
- **Closure helps to determine the normal forms of a relation:** By computing the closure of a set of FDs, we can identify the candidate keys and determine the appropriate normal form for the relation.


**Conclusion:**

Closure of a set of FDs is a fundamental concept in database systems. It helps to capture the implications of FDs, identify candidate keys, and ensure data integrity. Understanding closure is essential for database design and implementation.
