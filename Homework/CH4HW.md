# ISTA420 CH4 HW

1. In your own words, what is a subquery?  
A: A query within a query that grabs something more specific.
2. In your own words, what is a self contained subquery?  
A: It doesn't need the table from the query containing it. 
3. In your own words, what is a correlated subquery?  
A: It relies on the table referenced by the query containing it. 
4. Give an example of a subquery that returns a single value. When would you use this kind of subquery?  
A: Any scalar value subquery. 
5. Give an example of a subquery that returns multiple values. When would you use this kind of subquery?  
A: Any query using a parameter that belongs to multiple tables.
6. Give an example of a subquery that returns table values. When would you use this kind of subquery?  
A: Any kind of completed query that returns data.
7. What does the exists predicate do? Give an example.  
A: It returns a true or false value if targeted data exists. DROP TABLE IF EXISTS. 
8. What happens if we use the not operator before a predicate? Give an example.  
A: It looks for everything that is false within the predicate. Flips it.  
9. When you use exists or not exists with respect to a row in a database, does it return two or three
values? Explain your answer.  
A: 2, it only returns it exists or does not. 
