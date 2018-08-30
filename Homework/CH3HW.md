# ISTA 420 CH3 HW

1. In general, why would you even want to join two (or more) tables together? This is a good time to
think about the nature of relational algebra.  
A: You would join tables to access the relation between two area of information that might be related.
2. Describe in your own words the output from an inner join.  
A: You only get the matching rows, and discard the ones that don't match.
3. Describe in your own words the output from an outer join.  
A: Left outer joins merge the left rows, Right outer joins merge the right table and full outer joins match the rows that have a matching row and include the ones that come up null. 
4. Describe in your own words the output from an cross join.  
A: One table is essentially multiplied by the other row for row, creating a Cartesian product (all possible x, y's) You get all possible matches.
5. A convenient mnemonic for remembering the various joins is “Ohio.” Why is this true?  
A: One/Inner Hi/left, right, full One/cross
6. Give an example of a composite join.  
A: Where you need to join multiple attributes. 
7. What is the difference between the following two queries? The business problem is “How many orders
do we have from each customer?” 
================first query===============
SELECT C.custid, COUNT(*) AS numorders
FROM Sales.Customers AS C
LEFT OUTER JOIN Sales.Orders AS O
ON C.custid = O.custid
GROUP BY C.custid;  
================second query===============
SELECT C.custid, COUNT(O.orderid) AS numorders
FROM Sales.Customers AS C
LEFT OUTER JOIN Sales.Orders AS O
ON C.custid = O.custid
GROUP BY C.custid;  
A: The first one counts all of the rows. The second one counts rows with orderids. 
8. What might be one reason the following query does not return the column custID in this query?
SELECT C.custid, C.companyname, O.orderid, O.orderdate
FROM Sales.Customers AS C
LEFT OUTER JOIN Sales.Orders AS O
ON C.custid = O.custid
WHERE O.orderdate >= ’20160101’;  
A: Might not be an order date. 