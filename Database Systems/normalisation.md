## Normalization in Languages in Database Systems

### Introduction

Database normalization is a process of designing database tables to reduce data redundancy and improve data integrity. The goal is to minimize data anomalies, where inconsistencies and errors can occur due to duplicate data entry or improper data relationships. 

Normal forms are a set of rules that guide the process of database normalization. Higher normal forms ensure greater data integrity and efficiency.


### First Normal Form (1NF)

* Each record in the table represents a single entity.
* All attributes (columns) are atomic, meaning they contain only a single value. 
* Example: A table with student data including name, email, phone number, and address would be in 1NF.


### Second Normal Form (2NF)

* In addition to the requirements of 1NF, each non-key attribute should be dependent only on the primary key.
* Example: A table with student data and their grades would be in 2NF if the grades were only dependent on the student ID.


### Third Normal Form (3NF)

* Students in 3NF have non-key attributes that are fully dependent on the primary key, and every non-key attribute is dependent only on the primary key.
* Example: A table with student data and their course schedules would be in 3NF if the courses were linked to students through their IDs.


### Boyce-Codd Normal Form (BCNF)

* In BCNF, any non-key attribute is fully dependent on every subset of the primary key.
* Example: A table with student data and their grades would be in BCNF if the grades were dependent on both the student ID and the course ID.


### Fourth Normal Form (4NF)

* 4NF removes partial dependencies, where a non-key attribute is dependent on only part of the primary key.
* Example: A table with student data and their grades would be in 4NF if the grades were dependent on both the student ID and the course ID, but not on any individual parts of the student ID.


### Fifth Normal Form (5NF)

* In 5NF, the table is decomposed into a collection of tables such that there are no non-key attributes that are dependent on other non-key attributes.
* Example: A table with student data and their grades would be in 5NF if the students, courses, and grades were each stored in separate tables.


### Conclusion

Normalizing databases is an important process for maintaining data integrity and efficiency. By minimizing data redundancy and eliminating anomalies, organizations can improve the quality of their data and make it easier to manage.