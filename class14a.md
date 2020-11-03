##  Database Normalization
It is a process used to organize a database into tables and columns. 
The main idea with this is that a table should be about a specific topic and only supporting topics included.
Take a spreadsheet containing the information as an example, where the data contains salespeople and customers serving several purposes:

- Identify salespeople in your organization
- List all customers your company calls upon to sell a product
- Identify which salespeople call on specific customers.
> By limiting a table to one purpose you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications.

### Reasons for Database Normalization
There are three main reasons to normalize a database:
- The first: is to minimize duplicate data,
- the second : is to minimize or avoid data modification issues,
- and the third : is to simplify queries. 
### Data Duplication and Modification Anomalies
Notice that for each SalesPerson we have listed both the SalesOffice and OfficeNumber. There are duplicate salesperson data. Duplicated information presents two problems:
1- It increases storage and decrease performance.
2- It becomes more difficult to maintain data changes.
 ### Search and Sort Issues
 The last reason we’ll consider is making it easier to search and sort your data.  In the SalesStaff table if you want to search for a specific customer such as Ford, you would have to write a query like
 
### Definition of Database Normalization
There are three common forms of database normalization: 
- First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key

