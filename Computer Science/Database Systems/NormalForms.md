Path : [/Computer Science](../../index.md) [/Database Systems](../index.md)
## Normal Forms in Database Systems

**Introduction**

Database normalization is a process of organizing data in a way that minimizes redundancy and ensures data integrity. By applying normalization rules, we can reduce the risk of data inconsistencies and improve the efficiency of data management. There are several normal forms, each with its own level of data integrity and normalization.

**1NF (First Normal Form)**

- Each row in the table represents a single entity.
- Each column in the table represents an attribute of that entity.
- No repeating groups of data are allowed.


**Example:**

**Original Data:**

| Student Name | Address | Phone Number | Subjects |
|---|---|---|---|
| John Doe | 123 Main Street | 555-123-4567 | Math, Science |
| Jane Smith | 456 Oak Avenue | 555-234-5678 | English, History |


**Normalized Data:**

| Student Table | Address Table | Phone Table | Subjects Table |
|---|---|---|---|
| Student ID | Address ID | Phone Number | Subject ID |
| Name | Street | Number | Name |


**2NF (Second Normal Form)**

- In addition to fulfilling the requirements of 1NF, all non-key attributes must be functionally dependent on the primary key.
- No multi-valued dependencies exist.


**Example:**

**Original Data:**

| Employee ID | Name | Salary | Skills | Department |
|---|---|---|---|
| 1 | John Doe | 5000 | Writing, Design | IT |
| 2 | Jane Smith | 6000 | Marketing, Sales | Marketing |


**Normalized Data:**

| Employee Table | Skills Table |
|---|---|
| Employee ID | Skill ID |
| Name | Name |
| Salary | Department |


**3NF (Third Normal Form)**

- In addition to fulfilling the requirements of 1NF and 2NF, all non-key attributes are fully dependent on the primary key.
- There are no transitive dependencies.


**Example:**

**Original Data:**

| Customer ID | Name | Account Number | Balance | City |
|---|---|---|---|
| 1 | John Doe | 12345 | 100 | New York |
| 2 | Jane Smith | 23456 | 200 | London |


**Normalized Data:**

| Customer Table | Account Table | City Table |
|---|---|---|
| Customer ID | Account Number | Name |
| Name | Balance | City |


**Conclusion**

Normalizing data is an important process for maintaining data integrity and efficiency. By applying different normal forms, we can minimize data redundancy, reduce the risk of data inconsistencies, and improve the overall quality of our databases.
