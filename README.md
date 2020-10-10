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
  
</dl>


## Life without databases ➡️ issues
In the beginning, there were file-based systems with data stored in files. 

This type of system has problems with:
- __Data redundancy:__ same information kept in different files
- __Data isolation:__ difficult for new apps to find data
- __Concurrency:__ only one process can access a file at any given time

## Life with databases ➡️ 🎉

- __Support for multiple views:__ you can retrieve only the info you want and _only_ that info
- __Multiuser system__: Concurrency control strategies mean more than one person can access the database at a time
- __Data redundancy control__: Ideally, each data item is stored at _one place_ in the database
- __Integrity constraints__: Enforce data integrity by only allowing certain data in certain fields

### Credit

Notes from [Database Design](https://opentextbc.ca/dbdesign01/) and [Distributed systems for fun and profit](http://book.mixu.net/distsys/single-page.html).
