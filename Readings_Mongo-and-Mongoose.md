[Home](README.md)

# Readings: NODE.js

### Nosql vs SQL
---------------

Referenced the source below for answers<sup>1</sup>

Differences between NOSQL and SQL

a. *NOSQL* is a non-relational DBMS, or distrubuted database  *SQL* is a relational DBMS

b. *NOSQL* consists of documents, key-value pair, graph, or wide-column store databases  *SQL* consists of table based databases

c. *NOSQL* is a dynamic Schema *SQL* is a predefined Schema

d. *NOSQL* "Follows the Brewers CAP theorem (Consistency, Availability and Partition tolerance)" *SQL* "Emphasizes ACID properties (Atomicity, Consistency, Isolation and Durability)"<sup>1</sup>

e. *NOSQL* queries are focused on a large collection of documents with a varying syntax *SQL* queries use Structured Query Language to manipulating and defining data


1. What kind of data is a good fit for an SQL database?

  Data that involves complex queries

2. Give a real world example.

  "Grab the first 30 students who enrolled in any Bio-101 class who are juniors and return the result alphabetically, in ascending order". An SQl database may be a good choice here.

3. What kind of data is a good fit a NoSQL database?

  Hierarchical data or data that emulates key-value pairs

4. Give a real world example.

  "Return all the managers who work for regional manager X. From this return all the employees for each one work work in department Y". A NoSQL database may be a good choice here.

5. Which type of database is best for hierarchical data storage?

  NoSql

6. Which type of database is best for scalability?

  Both types work in different situations. SQL DBs scale vertically (manage load by improve specs) whereas NoSQl databases scale horizontally (manage load by up-ing serving count).


### Nosql vs SQL (video)
---------------

Referenced the source below for answers<sup>2</sup>

1. What does SQL stand for?
  Structured Query Language

2. What is a realational database?
  A database that works with SQL

3. What type of structure does a relational database work with?
  Tables and schemas

4. What is a ‘schema’?
  A defined set of requirments/constraints that model what a database should 'look' like.

5. What is a NoSQL database?
  A database where the data is not stored like a relational DB.There are no tables with records that follow a set of constraints and rules.

6. How does it work?
  Basically, data can have entries that have a different structure and/or different fields within the same logical group. Unlike a SQL DB, this is allowed.

7. What is inside of a Mongo database?
  Data is stored in collections rather than tables and these collections contain documents rather than records.

8. Which is more flexible - SQL or MongoDB? and why.
  MongoDB, it is 'schemaless'. Documents can be inserted in collections without following a set of rules to how that data should be formated.

9. What is the disadvantage of a NoSQL database?
  Not having a schema results in less data integrity.



### Things I want to know more about
---------------

* I would definetly want to see more examples of what sets of data would work better with SQL DBs vs NoSQL dbs (Performance considerations with large databases given specific sets of data with SQL vs NoSQL DBs)

* Querying MySQL and MongoDB databases in Node.js with the the mysql and mongoose libraries and how to appropiately handle scale with each.



###### Works Cited

<sup>1</sup> Issac, Luke _SQL vs NoSQL Database Differences Explained with few Example DB_, The Geek Stuff, Jan 14 2014, https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool

<sup>2</sup> "SQL vs NoSQL or MySQL vs MongoDB" YouTube, uploaded by Academin, July 15 2018, hhttps://www.youtube.com/watch?v=ZS_kXvOeQ5Y