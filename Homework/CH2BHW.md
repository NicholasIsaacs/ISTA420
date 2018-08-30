# ISTA 420 HW 2B

1. What is a data type? Why do we have data types?  
A: A classification that describes what type of data a variable has. 
2. What is a collation? Name four elements of a collation.  
A: Collation is a property of character data that lets you organize information based on characters found in foreign languages, accents and case. Four aspects: Latin1_General, Dictionary Sorting, CL, and AS. 
3. How would you strip whitespace from a string? For example, suppose you had “ Dave ” but
wanted only “Dave”.  
A: You could use the RTRIM LTRIM function. For example, RTRIM(LTRIM(' Dave '));
4. Suppose you wanted to make a list of every college and university that was called an Institute from
the college table. Write the query.  
A: SELECT name FROM college WHERE Name LIKE N'%Institute';
5. How would you find out the index of the first space in a string? For example, the index of the first
space in “Barack Hussein Obama” would be 7.  
A: CHARINDEX(" ", "Barack Hussein Obama")7
6. How would you select just the first name in a list of the presidents. Each record looks like the: ”George Washington”, ”John Adams”. First names can be an arbitrary length, from “Cal” to “Benjamin.” (e.g., Cal College, Benjamin Harrison)  
A: You would use the SUBSTRING function. SUBSTRING("George Washington", 1, CHARINDEX(" ","George Washington"))
7. What is the order of precedence for the logical operators?   
A:NOT, AND, BETWEEN IN LIKE ORDER
8. What is the order of precedence for the math operators?   
A: 1. () 2. *, /, % 3. +, -, |, ^ 4. <=> 5. NOT 6. AND 7. ALL, ANY, BETWEEN, IN, LIKE, OR, SOME 8.=
9. What is the difference between a simple and a searched CASE expression?   
A: Simple Case is used to match a value to a list of potential matches and returns the first matched value, while searched returns a value from the ELSE clause if there wasn't a match.
10. How would you turn a list of names like this: “LASTNAME, FIRSTNAME”, to a list like this:
A: SUBSTRING ("Wilson, Fabiola", CHARINDEX (" ", 'Wilson, Fabiola' )+1) SUBSTRING ("Wilson, Fabiola" CHARINDEX(","," Wilson, Fabiola")-1)   
11. How would you turn a list of names like this: “FIRSTNAME LASTNAME”, to a list like this: “LASTNAME,
FIRSTNAME”?  
A: SUBSTRING ("James Dix", CHARINDEX(" ", "James Dix")+1) SUBSTRING ("James Dix", 1, CHARDINDEX("))
