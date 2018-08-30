# CH.1  Background to T-SQL

1. How does the book describe the difference between imperative and declarative languages?
A: Imperative languages tell you how to get what you want, often in much detail while declaritive languages
tell you what you want without telling you how to get it. 

2. List three categories of command statements in SQL.
A: Data Definition Language (DDL), Data Manipulation Language (DML), Data Control Language (DCL)

3. Give an informal definition of database as used in the expression "relational database management
system." Give an informal definition of database as used in the expression "Human Resource database."
A: In the context of a relational database management system, a database is a system that operates and produces 
results based on parameters, that are set forth in the form of predicates, relations and propositions.
In the context of a human resource database, a database acts as a data entry and retrieval point similar to a log. 

4. How does SQL implement three-valued predicate logic?
A: Predicates in SQL can manifest as true, false, or null if the information is missing. Null essentially means
unknown because a lack of information makes a predicate neither true nor false. 

5. How does SQL enforce entity integrity? How does SQL enforce referential integrity?
A: SQL enforces entity integrity by using something called candidate keys. Candidate keys more or less act as
a unique indentifier for a row. SQL enforces referential integrity by using foreign keys. Foreign keys reference
in the same or possibly different candidate key. This acts as a constraint because it draws from the parameters
of another candidate key which lowers the possibilities of it matching both. 

6. What is a relation as defined in the textbook? A one word answer to this question is sufficient.
A:Set or table.

7. Is this table in first normal form? Why or why not? If it is not, how would you change it?
A: Yes, because all of the operations are unique and can not be broken down further. 

8. Is this table in second normal form? Why or why not? If it is not, how would you change it?
A: No, it is not. You can find all the information with either the owner id or pet id. To fix this
you should remove the pet id and make a table out of it with the dependent information. 

9. Is this table in third normal form? Why or why not? If it is not, how would you change it?
A: Yes, because all information is dependent upon the ID.

10. List the components of a four-part object name.
A: The schema name, object name, database name (prefix), and instance name (prefix).

11. What is the difference between declarative data integrity and procedural data integrity?
A: Declarative data integrity is enforced by table definition. Procedural data integrity is enforced by 
stored procedures. 
