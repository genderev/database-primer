# database-primer
Databases: the easy way.



## The basics

<dl>

  <dt>concurrency</dt>

  <dd>multiple users can access a record without anything bad happening</dd>

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
  
  
</dl>


## Life without databases ➡️ issues
In the beginning, there were file-based systems - data stored in files. 

This type of system has problems with:
- __Data redundancy:__ same information kept in different files
- __Data isolation:__ difficult for new apps to find data
- __Data integrity__
- __Security__
- __Concurrency:__ only one process can access a file at any given time



### Credit

Notes from [Database Design](https://opentextbc.ca/dbdesign01/) and [Distributed systems for fun and profit](http://book.mixu.net/distsys/single-page.html).
