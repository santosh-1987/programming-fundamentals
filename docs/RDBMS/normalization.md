# Data Normalization
DB Normalization is a technique that detects degree of redundancy(needless) of data in a database.
## Normal Forms
- 1NF (First Normal Form)
    - Each table cell should contain a single value.
    - Each record needs to be unique.
    - DB should not have multivalued columns
  ![img.png](../assets/images/rdbms/img.png)
  ![img_1.png](../assets/images/rdbms/img_1.png)
- 2NF (Second Normal Form)
  - Rule 1- Be in 1NF
  - Rule 2- Single Column Primary Key that does not functionally dependant on any subset of candidate key relation
  - ![img.png](../assets/images/rdbms/2nf.png)
- 3NF (Third Normal Form)
  - Rule 1- Be in 2NF
  - Rule 2- Has no transitive functional dependencies
- 3.5NF - BCNF (Boyce-Codd Normal Form)
- 4NF (Fourth Normal Form)
- 5NF (Fifth Normal Form)
- 6NF (Sixth Normal Form)

## Anomalies
- Update Anomaly
- Insert Anomaly
- Delete Anomaly


