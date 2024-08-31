

### What is a DATABASE?
A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS).

### What is DBMS?
Database Management Systems (DBMS) are software systems used to store, retrieve, and run queries on data. A DBMS serves as an interface between an end-user and a database, allowing users to create, read, update, and delete data in the database.

### DBMS vs RDBMS
The main difference between a DBMS(Database Management System) and an RDBMS(Relational Database Management system) is that a DBMS is a software application used to store, retrieve, and manage data in a database, while an RDBMS is a type of DBMS that stores data in a relational database.

### What is SQL?
Structured query language (SQL) is a programming language for storing and processing information in a relational database. A relational database stores information in tabular form, with rows and columns representing different data attributes and the various relationships between the data values.
Eg: oracle database, mySQL, Microsoft SQLServer, PostgresSQL

### What is nonSQL?
NoSQL, also referred to as “not only SQL”, “non-SQL”, is an approach to database design that enables the storage and querying of data outside the traditional structures found in relational databases.
eg:MongoDB, HBase, Neo4j, Cassandra, etc

### Difference between sql and non sql?
Type 
SQL databases are primarily called Relational Databases (RDBMS); whereas NoSQL databases are primarily called non-relational or distributed databases. 
Language 
SQL databases define and manipulate data-based structured query language (SQL). Seeing from a side this language is extremely powerful. SQL is one of the most versatile and widely-used options available which makes it a safe choice, especially for great complex queries. But from another side, it can be restrictive. SQL requires you to use predefined schemas to determine the structure of your data before you work with it. Also, all of your data must follow the same structure. This can require significant up-front preparation which means that a change in the structure would be both difficult and disruptive to your whole system. 
 
A NoSQL database has a dynamic schema for unstructured data. Data is stored in many ways which means it can be document-oriented, column-oriented, graph-based, or organized as a key-value store. This flexibility means that documents can be created without having a defined structure first. Also, each document can have its own unique structure. The syntax varies from database to database, and you can add fields as you go. 
Scalability 
In almost all situations SQL databases are vertically scalable. This means that you can increase the load on a single server by increasing things like RAM, CPU, or SSD. But on the other hand, NoSQL databases are horizontally scalable. This means that you handle more traffic by sharding, or adding more servers in your NoSQL database. It is similar to adding more floors to the same building versus adding more buildings to the neighborhood. Thus NoSQL can ultimately become larger and more powerful, making these databases the preferred choice for large or ever-changing data sets.
Structure 
 SQL databases are table-based on the other hand NoSQL databases are either key-value pairs, document-based, graph databases, or wide-column stores. This makes relational SQL databases a better option for applications that require multi-row transactions such as an accounting system or for legacy systems that were built for a relational structure. 
Property followed 
SQL databases follow ACID properties (Atomicity, Consistency, Isolation, and Durability) whereas the NoSQL database follows the Brewers CAP theorem (Consistency, Availability, and Partition tolerance). 
Support 
Great support is available for all SQL databases from their vendors. Also, a lot of independent consultants are there who can help you with SQL databases for very large-scale deployments but for some NoSQL databases you still have to rely on community support and only limited outside experts are available for setting up and deploying your large-scale NoSQL deploy. 
When To Use: SQL vs NoSQL 
SQL is a good choice when working with related data. Relational databases are efficient, flexible, and easily accessed by any application. A benefit of a relational database is that when one user updates a specific record, every instance of the database automatically refreshes, and that information is provided in real-time.
SQL and a relational database make it easy to handle a great deal of information, scale as necessary and allow flexible access to data only needing to update data once instead of changing multiple files, for instance. It’s also best for assessing data integrity. Since each piece of information is stored in a single place, there’s no problem with former versions confusing the picture.
 
While NoSQL is good when the availability of big data is more crucial, SQL is valued for ensuring data validity. It’s also a wise decision when a business needs to expand in response to shifting customer demands. NoSQL offers high performance, flexibility, and ease of use.
NoSQL is also a wise choice when dealing with large or constantly changing data sets, flexible data models, or requirements that don’t fit into a relational model. Document databases, like CouchDB, MongoDB, and Amazon DocumentDB, are useful for handling large amounts of unstructured data.



Major challenges 
1. writing efficient queries to retrieve information.
2. designing the schema, or structure, of the database.
3. understanding when to use advanced features.
4. managing the database in a production environment.


### ORM and ODM 
ORM (Object-Relational Mapping) and ODM (Object-Document Mapping) are both programming techniques that allow developers to interact with databases using object-oriented paradigms. However, they are used in different contexts: ORM is associated with relational databases, while ODM is associated with document databases.

ORM (Object-Relational Mapping):
Definition:
ORM is a programming technique that allows developers to interact with relational databases using objects in an object-oriented programming language. It facilitates the conversion between the relational model of a database and the object-oriented model of the application.
Use Case:
ORM is commonly used with relational databases like MySQL, PostgreSQL, or Oracle.
Key Concepts:
Tables in a relational database are mapped to classes in the application.
Rows in a table are mapped to instances (objects) of the corresponding class.
Relationships between tables are represented as associations between classes.
Example Frameworks:
Hibernate (Java)
Entity Framework (C#)
Django ORM (Python)
SQLAlchemy (Python)

ODM (Object-Document Mapping):
Definition:
ODM is a programming technique that allows developers to interact with document databases using objects in an object-oriented programming language. It facilitates the conversion between the document model of a database and the object-oriented model of the application.
Use Case:
ODM is commonly used with NoSQL document databases like MongoDB.
Key Concepts:
Collections in a document database are mapped to classes in the application.
Documents in a collection are mapped to instances (objects) of the corresponding class.
Embedded documents and arrays in documents are represented as nested objects and collections.
Example Frameworks:
Mongoose (Node.js, JavaScript)
Spring Data MongoDB (Java)
Morphia (Java)
Doctrine ODM (PHP)

Key Differences:
Data Model:
ORM deals with relational databases, where data is organized into tables with rows and columns.
ODM deals with document databases, where data is stored as flexible, JSON-like documents.
Flexibility:
Document databases, often used with ODM, offer more flexibility in the schema since each document in a collection can have different fields.
Relational databases, often used with ORM, have a more rigid schema with predefined tables and columns.
Examples:
ORM examples include Hibernate for Java and Entity Framework for C#.
ODM examples include Mongoose for Node.js and Spring Data MongoDB for Java.
Data Relationships:
In ORM, relationships between tables are typically represented using foreign keys.
In ODM, relationships between documents can be represented using references or embedded documents.
Query Language:
ORM typically uses SQL (Structured Query Language) for querying relational databases.
ODM uses query languages or methods specific to the document database, often based on JSON-like syntax.

In summary, ORM and ODM are techniques that help bridge the gap between the object-oriented programming world and different types of databases. ORM is associated with relational databases, while ODM is associated with document databases. The choice between ORM and ODM depends on the type of database being used in the application.



