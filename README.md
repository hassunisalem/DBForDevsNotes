# DBForDevsNotes


## The course focuses on five different database types:


### Relational databases

A relational database is a type of database that uses a structure 
that allows us to identify and access data in relation to another piece of data in the database.



### Column based databases

A column-oriented DBMS or columnar DBMS is a database management system (DBMS) that stores data tables by column rather than by row.



### Document databases

A document-oriented database, or document store, is a computer program and data storage system designed for storing, 
retrieving and managing document-oriented information, also known as semi-structured data. Documents can contain nested structures,
and so they exhibit a high degree of flexibility, allowing for variable domains.
The system imposes few restrictions on incoming data, as long as it meets
the basic requirement of being expressible as a document.



### Graph databases

In computing, a graph database (GDB) is a database that uses graph structures for semantic queries with nodes, edges, and properties to represent and store data.
 A key concept of the system is the graph (or edge or relationship).



### Key-value stores

A key–value database, or key–value store, is a data storage paradigm designed for storing, retrieving, and managing associative arrays, and a data structure more commonly known today as a dictionary or hash table.

Redis - gains amazing performance in exchange for increased risk of data loss in the case of a
hardware failure. 



## Additional notes




### PostgreSQL

PostgreSQL (or just “Postgres”) is a relational database management system
(or RDBMS for short).Relational databases are set-theory-based systems in
which data is stored in two-dimensional tables consisting of data rows and
strictly enforced column types.



### Single table

In this approach, all fields, which are defined under a super (parent) class, are stored in a single table. 
It is easy to query and retrieve different types from one table without need of join statements. 
However, a query to get Customer class object would also return irrelevant employeeNumber field; hence all regarding fields should be specified in the select statement.

Another problem is that, it is not possible to use constrains such as not null for a subclass. For example, customerNumber is an essential field for all Customer records. Yet applying not null constrain for customerNumber would prevent us from storing other objects without customerNumber such as Maintainer.


### ACID

Atomicity: Transactions are often composed of multiple statements. Atomicity guarantees that each transaction
is treated as a single "unit", which either succeeds completely, or fails completely: if any of the statements constituting a transaction fails to complete, the entire transaction fails and the database is left unchanged.

Consistency: Consistency ensures that a transaction can only bring the database from one valid state to another, maintaining database invariants: any data written to the database must be valid according to all defined rules, including constraints, cascades, triggers, and any combination thereof. 

Isolation: In database systems, isolation determines how transaction integrity is visible to other users and systems.

Durability: Durability guarantees that once a transaction has been committed, it will remain committed even in the case of a system failure (e.g., power outage or crash).


### Datamodel

views: ændre ikke på datamodellen (concurrency - der kan være mange clients der bruger views)

actions: ændre aktivt på datamodellen (cronlogisk rækkeføælge af clients der kører actions)

	Description: besrkivelse der bruges til dokumentation
	
	input: hvad der kommer ind i datamodellen og bliver parametre til metoden

	output: duh

	errorCodes: selvdefinerede fejlbeskeder

	

kinds: ses som tabeller med databseøjne, classser i java

