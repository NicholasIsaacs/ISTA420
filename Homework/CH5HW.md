# ISTA 420 CH5HW
1. What is a table expression? Can you give a technical definition of a table expression?  
A: A named expression that represents a valid relational table. A subquery that returns a table/multiple columns. 
2. In what SQL clause are derived tables (table valued subqueries) located?  
A: The from clause.
3. Why can you refer to column aliases in an outer query that you defined in an inner table valued
subquery?   
A: It runs the subquery first.
4. What SQL key word defines a common table expression?  
A: In-With expression
5. When using common table expressions, can a subsequent derived table use a table alias declared in a
preceding table expression?  
A: Yes
6. Can a main query refer to a previously defined common table expression by multiple aliases?  
A: Each cte represents a separate table that the machine retains the table.
7. In SQL, is a view a durable object?  
A: Yes, because it's stored as a permanent object.
8. In a view, what does WITH CHECK OPTION do? Why is this important?  
A: Prevents modification through the view that conflict with the view's filter.
9. In a view, what does SCHEMABINDING do? Why is this important?  
A: Binds the schema of referenced objects and columns to the schema of the referencing object. Referenced objects and columns can't be dropped.
10. What is a table valued function?  
A:  Reusable table expressions that support input parameters.
11. What does the APPLY operator do?  
A:  Applies the right table to each row from the left table and produces a result table with unified result sets.
12. What are the two forms of the APPLY operator? Give an example of each.  
A:  Cross Apply, Outer Apply. Cross apply, implements only one logical-query processing phase. Outer Apply implements two. 