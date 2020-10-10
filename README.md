# database primer 
Databases: the easy way.



## terms 📙

<dl>
  <dt>concurrency</dt>
  <dd>multiple users can access a record without anything bad happening</dd>
  <dt>concurrency control strategies</dt>
  <dd> the database lets multiple users see data at the same time while making sure that data is accurate </dd>
  <dt>data element</dt>
  <dd>single piece of info</dd>
  <dt>data inconsistency</dt>
  <dd>when copies of the same data contradict each other</dd>
  <dt>data isolation</dt>
  <dd>when and how changes made by one process become evident to other concurrent users or systems</dd>
  <dt>data integrity</dt>
  <dd>maintaining that data in the database is consistent and correct</dd>
  <dt> data redundancy </dt>
  <dd> when you have to update one value at multiple places </dd>
  <dt> database management system (DBMS) </dt>
  <dd> enables its users to create and control databases </dd>
  <dt> view </dt>
  <dd> subset of the database </dd>
  <dt> database constraint </dt>
  <dd> a restriction on what can be entered into a certain value for a data element </dd>
  <dt> data independence </dt>
  <dd> changing the organization of the database doesn't affect apps relying on the database </dd>
</dl>


## Life without databases ➡️ issues
In the beginning, there were file-based systems with data stored in files. 

This type of system has problems with:
- __Data redundancy:__ same information kept in different files
- __Data isolation:__ difficult for new apps to find data
- __Concurrency:__ only one process can access a file at any given time

## Benefits of databases

- __Support for multiple views:__ you can retrieve only the info you want and _only_ that info
- __Multiuser system__: Concurrency control strategies mean more than one person can access the database at a time
- __Data redundancy control__: Ideally, each data item is stored at _one place_ in the database
- __Integrity constraints__: Enforce data integrity by only allowing certain data in certain fields
- __Access control__: For security, different users have different levels of access to read and write for example
- __Transaction processing__: data is consistent and valid while multiple users perform the same transaction

## Data modeling

The first step of database design is to describe:
- the data contained in the database
- the relationships between data elements
- the database constraints for given data elements

## DBMS types

- __centralized:__ database and DBMS software stored at one site
- __distributed:__ database and DBMS software distributed through multiple sites
- __heterogenous distributed:__ different sites use different DBMS software, but they exchange info using additional software
- __multiuser:__ supports multiple users concurrently
- __single-user:__ does not support multiple users concurently 
- __object-oriented:__ DBMS represents info in the form of objects

## Relational databases

These are the most common databases, like Oracle and MySQL. They describe the world as “a collection of inter-related relations (or tables).”

- __table__: also known as relation or file; a database is composed of multiple tables and tables hold data
- __attribute__: another word to describe table columns; basic components of data into which your content can be broken down 
- __degree__: number of columns in a table
- __atomic value__: A piece of data in a database table that cannot be broken down any further
- __domain__: original sets of atomic values used to model data; set of acceptable values a column can contain
- __structured query language (SQL)__: most common language for accessing databases
- __tuple__: another way of saying _row_ or _record_
- __row:__ literally a row in the table; you could also say _record_

There's a lot of synonyms. Relation = table = file. Row = tuple = record. Column = attribute = field. [Normalization](https://dev.to/nexttech/database-normalization-explained-5b1a) is also important for relational databases. [This](https://github.com/8483/notes#database) is how you actually use MySQL.

## Object Relational Mapping

## N+1 Problem

## Sharding

## CAP Theorem

## ACID

## BASE

## CALM

## Convergent Replicated Data Types (CRDTs)

### Credit

Notes from: 
- [Database Design](https://opentextbc.ca/dbdesign01/) 
- [Distributed systems for fun and profit](http://book.mixu.net/distsys/single-page.html)
