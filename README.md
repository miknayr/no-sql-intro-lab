# NoSQL Research Lab

## Explainer
Up until now in the cohort we have stored data only in what are known as relational databases (SQL is the most well known type of relational DB querying language). Relational databases structure our data into tables. Today we will learn about a different type of database: a non-relational one. 

## Lab

In this lab you will be researching, either individually or in groups, answer to the following questions about noSQL databases. The intention is for you to spend some time learning about the fundamental differences between the type of databases we have seen before and the new type we will be learning about today. Even more importantly, you will learn about why two types of databases are used, and what situations fit each type of db. 

## Setup

Fork and clone this repository and answer questions as you research directly in the README. You do not have to submit this lab, but you will want to have it on hand for reference in the future. 

# Questions:
1. What does the term noSQL refer to, and what other term is often used synonymously with noSQL?
  - most agree that NoSQL databases are databases that store data in a format other than relational tables.
  - non SQL, or Not only SQL or non-relational databases.

2. What are some of the common arguments for using a non-relational versus a relational db?
  - flexible data models; 
      NoSQL databases typically have flexible schemas. allows you to easily make changes to your database as requirements change. can iterate quickly and continuously integrate new application features to provide value to your users faster.
  - horiztonal scaling;
      most SQL databases require you to scale-up vertically when you exceed the capacity requirements of your current server. conversely, most NoSQL databses allow you to scale-out horizontally, meaning you can add cheaper, commodity servers whenever you need them.

  - faster queries

  - easy for developers


3. In this class we will be using the document style of non-relational databases. What are the charecteristics of a document based db? 
  - Built around JSON-like documents, document databases are both natural and flexible for developers to work with.
  - intuitive data model;
    documents map to the objects in your code so theyre more natural to work with.

  - Flexible schema;
    fields can vary from document to document and you modify the structure at any time. maybe learn more about what this actually means

  - Universal;
    JSON documents are everywhere. Documents are a superset of all other data models so you can structure data any way your application needs – rich objects, key-value pairs, tables, geospatial and time-series data, and the nodes and edges of a graph.
  
  - Powerful;
  MongoDB comprehensive, and expressive. Ad hoc queries, indexing, and real time aggregations provide powerful ways to access, transform, and analyze your data.
  With ACID transactions you maintain the same guarantees you’re used to in SQL databases, whether manipulating data in a single document, or across multiple documents living in multiple shards.

  - Distributed;
  Unlike monolithic, scale-up relational databases, document databases are distributed systems at their core. Documents are independent units which makes it easier to distribute them across multiple servers while preserving data locality. Replication with self-healing recovery keeps your applications highly available while giving you the ability to isolate different workloads from one another in a single cluster. Native sharding provides elastic and application-transparent horizontal scale-out to accommodate your workload’s growth, along with geographic data distribution for data sovereignty. 


4. In this class we will be using Mongo specificially as our no-SQL db. Look into Mongo and answer this question: what is the priamry difference between how Mongo is maintained vrs SQL?
  - SQL databases are used to store structured data while NoSQL databases like MongoDB are used to save unstructured data. MongoDB is used to save unstructured data in JSON format. MongoDB does not support advanced analytics and joins like SQL databases support. 

5. Mongo DBs are organized into documents. Describe an example of a table in SQL that contains users, and then describe the equivalent DB setup in Mongo. 
- SQL stores data in tables, where columns are the attributes and rows are the value/property of the table. all these tables live inside databases.
- In MongoDB, data is stored in a collection, thats similar to MySQL tables. a collectiong consists of many documents in which data is stored in JSON format of key-value

basically each column is a collection and within each collection, the data inside is the rows?

ACID stands for Atomicity, Consistency, Isolation, and Durability. These properties focus on the consistency and reliability of the transaction done in the database. 



- In MySQL, the data is stored in tables, where the column denotes the attribute and row represents a particular record. These tables, in turn, reside inside the databases. In MongoDB, data is stored in collections that are analogous to MySQL tables. A collection can consist of many documents in which data is stored in JSON format of key-value. There can be hundreds of such collections inside a MongoDB database.

6. What is an example situation where a Mongo database makes sense versus a non-relational db?

I think a public list of cities, neighborhoods, streets that are publically known makes sense for a mongo DB vs a list of the home owners who opted into a program that identify themselves in the houses on the streets would be better for mySQL.
