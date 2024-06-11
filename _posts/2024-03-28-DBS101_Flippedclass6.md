---
Title: DBM101 Flipped Class 6
categories: [DBS101, Flipped_Class]
tags: [DBS101]
---

### Topic : Document type database ,Document type database ,Graph Database,Vector Database,Time Series Database,Column Oriented DataBase
---

## Document type database 

A document database is a type of NoSQL database that can be used to store and query data as JSON-like documents.

Popular document-oriented databases include MongoDB, DynamoDB and CosmosDB. MongoDB is one of the most popular examples of a document-oriented database. It includes features such as full index support, replication and sharding.

Documnent Database are used as:
Single view or data hub.
Customer data management and personalization.
Internet of Things (IoT) and time-series data.
Product catalogs and content management.
Payment processing.
Mobile apps.
Mainframe offload.
Operational analytics.

![alt text](/p1.png)

## Key Valued based Database

A key-value database is a type of non-relational database, also known as NoSQL database, that uses a simple key-value method to store data.

Examples of Popular Key-Value Databases:
Amazon DynamoDB: Probably the most widely used key-value store database, in fact, it was the research into DynamoDB that really started making NoSQL really popular. Aerospike: Open-source database that is optimized for in-memory storage.

Advantages:
It is very easy to use. ...
Its response time is fast due to its simplicity, given that the remaining environment near it is very much constructed and improved.
Key-value store databases are scalable vertically as well as horizontally.
Built-in redundancy makes this database more reliable.

![alt text](/key.png)

## Graph Database

Graph Database Defined. A graph database is defined as a specialized, single-purpose platform for creating and manipulating graphs. Graphs contain nodes, edges, and properties, all of which are used to represent and store data in a way that relational databases are not equipped to do.

Graph databases allow users to query linked data quickly and efficiently, making them much faster than traditional relational databases. With sophisticated algorithms and powerful search functions, graph databases can return complex query results across an interconnected network in milliseconds.

![alt text](/graph.png)

## Vector Database

A vector database is a collection of data stored as mathematical representations. Vector databases make it easier for machine learning models to remember previous inputs, allowing machine learning to be used to power search, recommendations, and text generation use-cases.

Vector database are used in AI like chatgpt as it can store text,voice and search in a large scalabe data.

Vector databases support flexible data models. They can handle structured and unstructured data, making them suitable for various applications, from text and image searches to recommendation systems. Efficiency: Vector databases are efficient in handling high-dimensional data.

Disadvantage for vector Database is data Type limitations.

## Time Series Database

Time series data is a set of values organized in the order in which they occur and arrive for processing.

Time series databases are designed to handle large volumes of incoming data points that arrive at a high frequency. They are optimized for high write throughput, which means they can ingest and store large amounts of data quickly and efficiently, in real time.

Use cases for time-series databases
Monitoring software systems and bare-metal hardware systems.
Continually capturing metrics from internet of things (IoT) devices.
Financial trading systems.
Recording stock prices over time.
Asset-tracking applications.

Disadavntage for time series database :
Time series data analysis does not support the missing values.
The analysis may lead to inaccurate results in the long term.

## Column Oriented DataBase

Column oriented database is s a type of database management system (DBMS) that stores data in columns together on disk. This enables faster queries for data analytics, which generally involves filtering and aggregating table columns.

Columnar databases offer a solution by addressing pain points such as improved query speed, enhanced compression, and efficient analytics, revolutionizing data storage and retrieval. A columnar database stores data in columns rather than rows, optimizing query performance for efficient retrieval and analysis.

Disadvantages of Column Store Databases:
Limited write performance
