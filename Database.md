# Database

**1.  Types**

Find out what the difference in the types. How to pick which DB to use (write-heavy vs read heavy, type/structure of data to be stored, etc)

* SQL - RDBMS(MySQL, PostgreSQL**)
* NoSQL - MongoDB

Useful Links:

   * https://medium.com/must-know-computer-science/system-design-sql-vs-nosql-4cdfb9f53d69
   
**2.  Core Concepts**

Useful Links:

   * https://www.geeksforgeeks.org/acid-properties-in-dbms/
   * https://www.geeksforgeeks.org/sql-ddl-dql-dml-dcl-tcl-commands/ 
   * https://www.w3schools.in/dbms/database-normalization/
   * https://en.wikipedia.org/wiki/Database_normalization
   * https://www.guru99.com/database-normalization.html
  
* SQL Queries - Syntax, Joins, Conditionals (where)       
* Transactions:
    * Commit
    * Rollback
* ACID 
    * Atomicity
    * Consistency
    * Isolation
    * Durability
* Database normalization and normal forms    
* DDL – Data Definition Language
* DQl – Data Query Language
* DML – Data Manipulation Language
* DCL – Data Control Language
* Database constraints - Primary key, Foreign key, Unique
* SQL Injection
* Database engines** - MyiSam etc    
 
**3.  SQL Datatypes** 

Useful links:

   * https://www.w3schools.com/sql/sql_datatypes.asp 
   * https://www.journaldev.com/16774/sql-data-types
   * https://www.javatpoint.com/sql-data-types
    

**4.  DB Optimization/Performance/Redundancy Techniques**   

Useful Links:

   * https://wizardzines.com/comics/indexes/
   * https://roadmap.sh/guides/scaling-databases
   
Techniques: 
   
* Indexing
* Data partitioning - Vertical vs Horizontal
* Sharding
* Data replication - Master-Slave database architecture (Reading and writing from different)
* Backups
* Regular DB Cleanup - Lazy cleanup(After user request) vs Active(Scheduled e.g daily via CRON job)
    
**5.  Other Concepts/Technology**    

* Database versioning/migration tools (e.g Flyway)
* UUID vs Long in IDs(Primary Keys) - Guarantee confidentiality
* Connection pool - Why we use it. Advantages,
* SQL queries patterns and anti-patterns e.g:
    - Avoid searching with “like”.
    - Have an index on the columns you are using for conditions (where x = y).  
    - At application level use connection pool (avoid huge no, minimize idle pool connection)to avoid cpu wait time 
    - Avoid 'order by' at DB level; try ordering on the application.
    - Limit records 5. Select only required rows (avoid * )
    - Paginate