Path : [/Computer Science](<..\..\index.md>) [/Database Systems](<..\index.md>)
## Normalization Techniques in Data Modeling in Database Systems

**Introduction**

Data normalization is a process of organizing data in a database to reduce data redundancy and improve data integrity. By eliminating data duplication and minimizing redundancy, normalization enhances efficiency, simplifies data management, and promotes data consistency.


**1NF - First Normal Form**

- Ensures unique identification for each record.
- Each field in the table should contain atomic values (indivisible).


**Example:**

**Raw Data:**

| ID | Name | Address | Age | City |
|---|---|---|---|---|
| 1 | John Doe | 123 Main Street | 25 | New York |
| 2 | Jane Smith | 456 Oak Avenue | 30 | London |

**Normalized Data:**

| ID | Name | AddressID | Age | City |
|---|---|---|---|---|
| 1 | John Doe | 1 | 25 | New York |
| 2 | Jane Smith | 2 | 30 | London |

**2NF - Second Normal Form**

- Meets all the requirements of 1NF.
- Further eliminates partial dependencies, where a non-key attribute depends on only part of the primary key.


**Example:**

**Raw Data:**

| StudentID | Name | Course | Grade |
|---|---|---|---|
| 1 | John Doe | Math | A |
| 1 | John Doe | Science | B |
| 2 | Jane Smith | Math | C |

**Normalized Data:**

| StudentID | Name | |
|---|---|
| 1 | John Doe | |
| 2 | Jane Smith | |

| CourseID | CourseName |
|---|---|
| 1 | Math |
| 2 | Science |

| StudentCourseID | StudentID | CourseID | Grade |
|---|---|---|---|
| 1 | 1 | 1 | A |
| 2 | 1 | 2 | B |
| 3 | 2 | 1 | C |


**3NF - Third Normal Form**

- Meets all the requirements of 1NF and 2NF.
- Data is further normalized by ensuring that no non-key attribute depends on another non-key attribute.


**Example:**

**Raw Data:**

| Employee | Manager | Salary | Department | Location |
|---|---|---|---|---|
| John Doe | Jane Smith | 5000 | Sales | New York |
| Jane Smith | Peter Jones | 6000 | Marketing | London |

**Normalized Data:**

**Employees:**

| EmployeeID | Name | Email |
|---|---|---|
| 1 | John Doe | john.doe@example.com |
| 2 | Jane Smith | jane.smith@example.com |
| 3 | Peter Jones | peter.jones@example.com |

**Managers:**

| ManagerID | Name | Email |
|---|---|---|
| 1 | Jane Smith | jane.smith@example.com |
| 2 | Peter Jones | peter.jones@example.com |

**Departments:**

| DepartmentID | Name | Location |
|---|---|---|
| 1 | Sales | New York |
| 2 | Marketing | London |

**Conclusion**

Normalizing data is an iterative process that improves data integrity, minimizes redundancy, and enhances the efficiency of data management in a database system. The level of normalization required depends on the specific needs of the organization and the nature of the data being stored.
