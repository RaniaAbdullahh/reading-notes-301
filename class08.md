
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
 Since the DISTINCT keyword will blindly remove duplicate rows, we will learn in a future lesson how to discard duplicates based on specific columns using grouping and the GROUP BY clause.
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

- OUTER JOINs:
Depending on how you want to analyze the data, the INNER JOIN we used last lesson might not be sufficient because the resulting table only contains data that belongs in both of the tables.

- NULLs
NULL values in an SQL database. It's always good to reduce the possibility of NULL values in databases because they require special attention when constructing queries, constraints
- Multi-table queries with JOINs:
Using the JOIN clause in a query, we can combine row data across two separate tables using this unique key. The first of the joins that we will introduce is the INNER JOIN.

