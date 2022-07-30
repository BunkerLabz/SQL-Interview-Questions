# SQL Interview Questions & Answers

Comprehensive Guide To Interviews For SQL

###  What is a database?

A database is described as an organized way of collection of DATA. It is the collection of schemes, tables, queries, reports, views and other objects.

```SQL
CREATEDATABASE DB_Name
```
### What is Relational Database Management System (RDMBS)?

RDBMS store data into a collection of tables, which is related by common fields between the columns of the table. It also provides relational operators to manipulate the data stored into the tables.

### What is Structured Query Language?

SQL stands for Structured Query Language, and it is used to communicate with the Database. This is a standard language used to perform tasks such as retrieval, updates, insertion and deletion of data from a database.

### What is primary key?

A primary key is a combination of fields which uniquely specify a row. This is a special kind of unique key, and it has implicit NOT NULL constraint. This means, Primary key values cannot be NULL.

### What is a unique key?

A Unique key constraint uniquely identifies each record in a database. This provides uniqueness for the column or set of columns. A Primary key constraint has automatic unique constraint defined on it. There can be many unique constraints defined per table, but only one Primary key constraint defined per table.

### What is the difference between Primary key and unique key?
Primary key does not allow the null values but unique key allows one null value.

Primary key will create clustered index on column but unique key will create non-clustered index by default.

### What is a foreign key?

A foreign key is one table which can be related to the primary key of another table. Relationships need to be created between two tables by referencing the foreign key with the primary key of another table.

### Explain the difference between spreadsheets and databases.

 * **Spreadsheet:**
A file that exists of cells in rows and columns and can help arrange, calculate and sort data. It can have numeric values, text, formulas and functions. It features columns and rows to keep inserted information legible and simple to understand. It is an electronic graph sheet.

* **Database:**
It is an organized collection of data arranged for ease and speed of search and retrieval. It contains multiple tables. A database engine can sort, change or serve the information on the database. Basically, it is a set of information which is held in a computer.

### What are the various SQL languages.

There are five types of SQL commands: DDL, DML, DCL, TCL, and DQL.

### What is Data Definition Language (DDL)?

DDL changes the structure of the table like creating a table, deleting a table, altering a table, etc. All the commands of DDL are auto-committed which means that it permanently saves all the changes in the database.
Some commands that come under DDL:
> CREATE, ALTER, DROP, TRUNCATE

### What is Data Manipulation Language (DML)?

DML commands are used to modify the database. It is responsible for all forms of changes in the database. The commands of DML are not auto-committed which means that it can't permanently save all the changes in the database.
Some commands that come under DML:
> INSERT, UPDATE, DELETE

### What is Data Control Language (DCL)?

DCL commands are used to grant and take back authority from any database user.
Some commands that come under DCL:
> Grant, Revoke

### What is Transaction Control Language (TCL)?

TCL commands can only be used with DML commands like INSERT, DELETE and UPDATE. These operations are automatically committed in the database, which is why they cannot be used while creating tables or dropping them. 
Some commands that come under TCL:
> COMMIT, ROLLBACK, SAVEPOINT

### What is Data Query Language (DQl)?

DQL is used to fetch the data from the database. 
It uses only one command:
> SELECT

### What is normalization?

Normalization is the process of minimizing redundancy and dependency by organizing fields and tables of a database. The main aim of Normalization is to add, delete or modify fields that can be made in a single table.

### Explain the different types of normalization.
* **Some types are:**
  * **First Normal Form (1NF):** This should remove all the duplicate columns from the table. Creation of tables for the related data and identification of unique columns.
  
  * **Second Normal Form (2NF):** Meeting all requirements of the first normal form. Placing the subsets of data in separate tables and Creation of relationships between the tables using primary keys.
  
  * **Third Normal Form (3NF):** This should meet all requirements of 2NF. Removing the columns which are not dependent on primary key constraints.
  
  * **Fourth Normal Form (4NF):** Meeting all the requirements of third normal form and it should not have multi-valued dependencies.

### What is denormalization?

Denormalization is a technique used to access the data from higher to lower normal forms of database. It is also a process of introducing redundancy into a table by incorporating data from the related tables.

### What is join?

This is a keyword used to query data from more tables based on the relationship between the fields of the tables. 

### Explain different types of join?

* **Left Outer Join:** If we want all the records from left table and only matching records from right table then will use left outer join/left join.

* **Right Outer Join:** If we want to display all the records from right table and only matching records from left table then will right outer join/right join.

* **Full Outer Join:** If we want to display all the records from both the tables then will use full outer join.

* **Inner Join:** If we want only the matching records from both the tables then will use Inner join/Simple join.

### What are the different types of indexes?

An index is a performance tuning method of allowing faster retrieval of records from the table. An index creates an entry for each value and makes it faster to retrieve data.
There are three types of indexes:
* **Unique Index:** This indexing does not allow the field to have duplicate values if the column is unique indexed. Unique index can be applied automatically when primary key is defined.

* **Clustered Index:** This type of index reorders the physical order of the table and search based on the key values. Each table can have only one clustered index.

* **Non-Clustered Index:** Non-Clustered Index does not alter the physical order of the table and maintains logical order of data. Each table can have 999 non- clustered indexes.

### What is query?

A DB query is a code written in order to get the information back from the database. Queries can be designed in such a way that it matches with our expectation of the result set.

### What is a subquery?

A subquery is a query within another query. The outer query is called as main query, and inner query is called subquery. SubQuery is always executed first, and the result of subquery is passed on to the main query.
There are two types of sub-queries: Correlated and Non-Correlated.
* **Correlated Subquery:** A correlated subquery cannot be considered as an independent query.

* * **Non-Correlated Subquery:** A Non-Correlated sub query can be considered as independent query and the output of subquery are substituted in the main query.

### Differentiate between the DELETE and TRUNCATE commands.

**DELETE** command is used to remove rows from the table, and WHERE clause can be used for conditional set of parameters. Commit and Rollback can be performed after delete statement.

**TRUNCATE** removes all rows from the table. Truncate operation cannot be rolled back.

### What are local and global variables?

**Local variables** are the variables which can be used or exist inside the function. They are not known to the other functions and those variables cannot be referred to or used. Variables can be created whenever that function is called.

**Global variables** are the variables which can be used or exist throughout the program. Same variable declared in global cannot be used in functions. Global variables cannot be created whenever that function is called.

### What is the difference between DROP and TRUNCATE statements?

**TRUNCATE** removes all the rows from the table, and it cannot be rolled back.

**DROP** command removes a table from the database and operation cannot be rolled back.

### What are constraints?

Constraint can be used to specify the limit on the data type of table. Constraint can be specified while creating or altering the table statement.

### What is data integrity?

Data Integrity defines the accuracy and consistency of data stored in a database. It can also define integrity constraints to enforce business rules on the data when it is entered into the application or database.

### What is auto increment?

Auto increment keyword allows the user to create a unique number to be generated when a new record is inserted into the table. 
AUTO INCREMENT keyword can be used in Oracle and IDENTITY keyword can be used in SQL SERVER.

### What are aggregate and scalar functions?
Functions are methods used to perform data operations. SQL has many in-built functions used to perform string concatenations, mathematical calculations etc.
SQL functions are categorized into the following two categories: Aggregate Functions and Scalar Functions.
* **Aggregate SQL Functions**
The Aggregate Functions in SQL perform calculations on a group of values and then return a single value. Following are a few of the most commonly used Aggregate Functions:
```SQL
| **Function**      | **Descreption**      |
| ------------- | ------------- |
| SUM()          | The SUM() function returns the total sum of a group of values.         |
| COUNT()           | The COUNT() function returns the number of rows in a database table.         |
| AVG()           | The AVG() function calculates the average of a set of values.         |
| MIN()           | The MIN() function returns the lowest value in a set of values.         |
| MAX()           | The MAX() function returns the highest value (maximum) in a set of values.         |
| FIRST()           | Test2         |
| LAST()           | Test2         |
```

* **Scalar SQL Functions**
The Scalar Functions in SQL are used to return a single value from the given input value. Following are a few of the most commonly used Scalar Functions:

```SQL
| **Function**      | **Descreption**      |
| ------------- | ------------- |
| UCASE()           | The UCASE() or upper case function will change the case of the string to upper case characters.         |
| LCASE()           | The LCASE() or lower case function will change the case of the string to lower case characters.         |
| MID()           | The MID() function is used to extract substrings from the table's column, which contain values of string type.         |
| LENGTH()           | The LENGTH() function returns the length of the string in the column.         |
| ROUND()           | The ROUND () function is used to round a numeric column to the number of decimals specified.         |
| NOW()           | NOW() function returns the current system's date and time.         |
| FORMAT()           | The FORMAT () function is used to format how a column is to be displayed.         |
```

