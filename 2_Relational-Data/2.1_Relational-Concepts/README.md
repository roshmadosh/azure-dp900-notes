### Identify features of relational data
A relational database is composed of tables, or **entities**. Examples of entities are products, customers, and orders for an e-commerce application.   

Entities have a defined schema. That is, any row added to an entity must conform to a structure, and declare values for each attribute (i.e. column) in the entity of the appropriate data type.  

### Describe normalization and why it is used
**Normalization** is a way of designing a schema (i.e. a way of defining your tables) such that you are less prone to duplicating data, and your entities are less likely to be in an "inconsistent" state (e.g. an order has a customer who's record was deleted from the Customers entity). A relational database staying in a "consistent" state is also called _maintaing referential integrity_.

There are several levels of normalization (called _forms_ of normalization), and each level can be thought of as adding a layer of "normality" to your schema design. A table in _third normal form_ is considered the minimal level of normality you want to achieve.  

Azure's docs generalize the process of normalization as requiring the following things:
- separate each entity into its own table
- separate each distinct attribute into its own column
- have a primary key for each table that uniquely identifies each row
- use foreign keys to relate tables to each other  

### Identify common structured query language (SQL) statements
**Data Definition Language** (DDL) is for creating, modifying, and removing entire tables from a relational database. The most commonly used SQL commands are CREATE, DROP, ALTER, RENAME.  

**Data Control Language** (DCL) is for managing access to database resources. The most common SQL commands are GRANT, DENY, and REVOKE.

**Data Manipulation Language** (DML) is used for manipulating rows in tables. The common SQL commands are SELECT, INSERT, UPDATE, and DELETE. WHERE is used to filter rows and JOIN is used to combine rows and columns from separate tables.  

### Identify common database objects
A **View** in a relational database is used to describe the result of a query. As the name indicates, query results are transient and don't actually create new tables in the database.  

A **stored procedure** is logic that's intended to be performed repeatedly. Stored procedures can be parameterized to expand their capabilities. 

An **index** is a way to make read queries based on a certain column faster at the expense of making insert or delete operations more costly. If you frequently make queries based on a non-primary-key attribute, it may be a good idea to add an index to that column. Adding an index to a table doesn't come for free, as indices take up space in memory and make other, non-read queries more expensive.  
