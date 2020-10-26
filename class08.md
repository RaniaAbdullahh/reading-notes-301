
## What is SQL?
> SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

### here are many popular SQL databases
-  SQLite
- MySQL
- Postgres
- Oracle 
- Microsoft SQL Server

### Relational databases
collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.
- ex : 

|Id	|Make/Model	|# Wheels	|# Doors |	Type        |
|---|-----------|---------|--------|--------------|
|1	|Ford Focus	|4	      |4   	   |Sedan         |
|2	|Tesla      |Roadster	|4	     |2	|Sports     |
|3	|Kawakasi   |Ninja   	|2	     |0	|Motorcycle |
|4	|McLaren    |Formula  |1	     |4	|Race       |

---------
-  SELECT queries
``SELECT column1, 2, …
FROM mytable;``
- ueries with constraints
``SELECT column, another_column, …
FROM mytable
WHERE condition
    AND/OR another_condition
    AND/OR …;``
    
 - Filtering and sorting Query results
 `` SELECT DISTINCT column, another_column, …
FROM mytable
WHERE condition(s);`` 
- Multi-table queries with JOINs
``SELECT column, another_table_column, …
FROM mytable
INNER JOIN another_table 
    ON mytable.id = another_table.id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;``
-  OUTER JOINs
`` SELECT column, another_column, …
FROM mytable
INNER/LEFT/RIGHT/FULL JOIN another_table 
    ON mytable.id = another_table.matching_id
WHERE condition(s)
ORDER BY column, … ASC/DESC
LIMIT num_limit OFFSET num_offset;``
    
