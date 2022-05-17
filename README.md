# NoSQL DATABASES FOR BETTER PERFORMANCE AND SCALING
![NoSql](https://media.istockphoto.com/photos/structured-query-language-database-technology-concept-nosql-picture-id1288398069?k=20&m=1288398069&s=612x612&w=0&h=_smTJUj70JKd5h-AKTYBNBRquk9lBc-X9CJ7yQlw5ek=)
## Abstract
This paper is about usage of NoSQL databases for better performance and scaling in any projects and types of NoSQL databases, What is the use of every database, how it works and how every database will be useful to a project. Finally concluding which database is best or  better.

## Introduction
### NoSQL database:
  - NoSQL databases (aka "not only SQL") are non-tabular databases and store data differently than relational tables.
  - NoSQL databases come in a variety of types based on their data model. 
  - The main types are **document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads**.
  - “NoSQL” also stands for “non SQL” while others say it stands for “not only SQL.” Either way, mostly NoSQL databases are databases that store data in a format other than relational tables.
  - NoSQL databases have a dynamic schema that is much better suited for big data as flexibility is an important requirement. Also, large amounts of analytical data can be stored in NoSQL databases for predictive analysis. An example of this is data from various social media sites such as Instagram, Twitter, Facebook, etc.

## Why NoSQL DB's are better than Relational DB's
### Relational database:
- A relational database is a type of database that stores and provides access to data points that are related to one another. Relational databases are based on the **relational model, an intuitive, straightforward way of representing data in tables**.
- A relational database includes tables containing rows and columns.
  
  ![click here](https://insightsoftware.com/wp-content/uploads/2022/02/dog_relational_database-1.png) **example of data storage in form of tables in relational database and link between tables**.

  **NoSQL databases don't require any predefined schema, allowing you to work more freely with “unstructured data.” Relational databases are vertically scalable, but usually more expensive, whereas the horizontal scaling nature of NoSQL databases is more cost-efficient**.

## Types of NoSQL DB's
1. ### Wide-column store
2. ### Document store
3. ### Key-value store
4. ### Graph store
5. ### Multi-model

## 1.Wide-column store
A wide column database, or wide column store, is a type of NoSQL database that stores data across flexible columns. These columns can then be stored across multiple servers or database nodes.
![wide_column_database](https://www.openlogic.com/sites/default/files/image/2021-08/wide%20column%20database%20example.JPG) **Wide column database example showing unique column labels by row**
### Work process : 
Similar to relational databases, wide column databases organize data into columns. But that’s where most of the practical similarities end. Wide column databases like Cassandra and Hadoop (HBase) are built with scale in mind, and they can store distributed, partitioned columns of data.
Columns are also treated differently in wide column databases, with the capacity for multiple column formats and names across rows. Because of how the data is accessed and stored, it also allows for higher compression of data and the facilitation of large volumes of data.
### Usage of wide Column Database
Common usage of wide-column databases favor those that **write a large amount of non-structured data, including logging and reporting systems, time series data, and user preference data**.
Use cases that require immediate data consistency are not a good fit for wide column databases like Cassandra, as, generally, they are eventually consistent, but not immediately consistent across all places where the data is held.

## 2.Document store
The document-oriented databases or NoSQL document store is a modernised way of storing data as JSON rather than basic columns/rows i.e. storing data in its native form.
This storage system lets you retrieve, store, and manage document-oriented information, it’s a very popular category of modern NoSQL databases, used by the likes of MongoDB, Cosmos DB, DocumentDB, SimpleDB, PostgreSQL, OrientDB, Elasticsearch and RavenDB.
### Documents are easier to work with than tables
Document databases use practical, intuitive modelling that reads faster than relational models. If you add superior indexing, this is boosted further.
Many developers choose Oracle and SQL over NoSQL because they think rows and columns read faster than documents. Document databases have been consuming more of the market share once occupied by relational databases because developers are wizening up to the truth.
![document_database](https://www.kdnuggets.com/wp-content/uploads/williams-document-dbs-0.jpg) 

**Comparision between relational model and document store model**

Relational databases would be faster if all the info needed per query was contained in a single row. In reality, the query has to search across several locations, retrieving data nested across different tables, then piecing it back together before spitting out the result. Whereas document databases contain all the data you need one location. All you need to do is query it, massively reducing complexity and boosting performance.

## 3.Key-value store
A key-value database is a type of nonrelational database that uses a simple key-value method to store data. A key-value database stores data as a collection of key-value pairs in which a key serves as a unique identifier. Both keys and values can be anything, ranging from simple objects to complex compound objects.

![key_value_store](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTNiblJEONPX-HG-6LmMLR7cOumS9-SKliS_9BarjWPwdHu8XvYqUUmKXgvMTiYjbUsUIU&usqp=CAU)
![key_value_store_2](https://redis.com/wp-content/uploads/2020/10/key-value-figure-a.png)

### Key-value store advantages
There are a few advantages that a key-value store provides over traditional row-column-based databases. Thanks to the simple data format that gives it its name, a key-value store can be very fast for read and write operations. And key-value stores are very flexible, a valued asset in modern programming as we generate more data without traditional structures.
Also, key-value stores do not require placeholders such as “null” for optional values, so they may have smaller storage requirements, and they often scale almost linearly with the number of nodes.
### Key-value database usage
- Web applications may store user session details and preference in a key-value store. All the information is accessible via user key, and key-value stores lend themselves to fast reads and writes.
- Real-time recommendations and advertising are often powered by key-value stores because the stores can quickly access and present new recommendations or ads as a web visitor moves throughout a site.
- On the technical side, key-value stores are commonly used for in-memory data caching to speed up applications by minimizing reads and writes to slower disk-based systems. Hazelcast is an example of a technology that provides an in-memory key-value store for fast data retrieval.

## 4.Graph store
A graph database is defined as a specialized, single-purpose platform for creating and manipulating graphs. Graphs contain nodes, edges, and properties, all of which are used to represent and store data in a way that relational databases are not equipped to do.
Graph analytics is another commonly used term, and it refers specifically to the process of analyzing data in a graph format using data points as nodes and relationships as edges. Graph analytics requires a database that can support graph formats; this could be a dedicated graph database, or a converged database that supports multiple data models, including graph.
### How graphs and graph databases work?
Graphs and graph databases provide graph models to represent relationships in data. They allow users to perform “traversal queries” based on connections and apply graph algorithms to find patterns, paths, communities, influencers, single points of failure, and other relationships, which enable more efficient analysis at scale against massive amounts of data. The power of graphs is in analytics, the insights they provide, and their ability to link disparate data sources.

When it comes to analyzing graphs, algorithms explore the paths and distance between the vertices, the importance of the vertices, and clustering of the vertices. For example, to determine importance algorithms will often look at incoming edges, importance of neighboring vertices, and other indicators.

Graph algorithms—operations specifically designed to analyze relationships and behaviors among data in graphs—make it possible to understand things that are difficult to see with other methods. When it comes to analyzing graphs, algorithms explore the paths and distance between the vertices, the importance of the vertices, and clustering of the vertices. The algorithms will often look at incoming edges, importance of neighboring vertices, and other indicators to help determine importance. For example, graph algorithms can identify what individual or item is most connected to others in social networks or business processes. The algorithms can identify communities, anomalies, common patterns, and paths that connect individuals or related transactions.

Because graph databases explicitly store relationships, queries and algorithms utilizing the connectivity between vertices can be run in sub-seconds rather than hours or days. Users don’t need to execute countless joins and the data can more easily be used for analysis and machine learning to discover more about the world around us.
![graph_store](https://www.oracle.com/a/ocom/img/cc01-graph-database-relationships.jpg)
### Graph database use cases:
- Money laundering
- Social media analysis
- Credit card fraud

(Look into **References** section for more details)

## 5.Multi-model
A multi-model database is a management system that combines multiple database types with a single backend. Most database management systems support only a single database model. On the other hand, multi-model databases store, query, and index data from different models.

Multi-model databases provide the modeling advantages of polyglot persistence without having to find ways to combine different models. The flexible approach allows storing data in different ways. The result is:
    Agile and flexible programming.
    Reduced data redundancy.

For example, exploring relationships between data points or building a recommendation system is much easier with graph databases. On the other hand, relational databases help define relationships between columns of data.

A vital multi-model database feature is the ability to transform data from one format to another. For example, data in JSON format quickly transforms into XML. Converting data formats provides additional agility and makes it easier to fulfill specific project requirements.

### Multi-Model Database Use Case Examples

Use cases help provide an idea of how multi-model databases work. Analyzing practical examples provide better insight into how multiple models work together in one system.

**1. Storing and Managing Multiple Data Sources**

A typical IT system uses various data sources. The stored information is not always in the same format or database. Multiple formats create a complex system, making it hard to maintain and search through data.

Storing data in a multi-model database makes administration easier. Everything is in one database, which reduces the time needed to store and manage data from different sources.

**2. Extending Model Features**

Multi-model databases provide extensions between models. Features from some models help supplement the shortcomings of other models.

For example, querying data in JSON format using SQL queries is simple. There is no need to adjust the original data source. Extensibility reduces data processing time and eliminates the need for extract, transform and load (ETL) systems.

**3. Hybrid Data Environments**

A typical data environment keeps operational data separate from analytical. The data for analysis must be transformed and stored in a different place from the operational data.

The information duplicates, decreasing data quality. Likewise, the separated space creates maintenance overhead. Both databases need policy administration as well as backup management.

A multi-model database provides a hybrid approach to data storage. A unified data hub for storing transactional and extracting analytical data is simpler to maintain.

### The Best Multi-Model Databases:
There are many different multi-model database types available on the market. The one distinguishable feature is the support for multiple models in one backed engine.
- MarkLogic Server
- ArangoDB
- OrientDB

## Conclusion
There are a wide variety of database modeling techniques exist, each providing a unique solution with benefits and drawbacks. Multi-model databases attempt to unify various databases into a single backend, reducing complexity and overhead as a system expands.

## References
- [Types of NoSQL databases](https://www.blazeclan.com/blog/dive-deep-types-nosql-databases/)
- [wide column database](https://www.openlogic.com/blog/guide-open-source-wide-column-databases)
- [Document store](https://ravendb.net/articles/nosql-document-oriented-databases-detailed-overview)
- [Key Value store](https://hazelcast.com/glossary/key-value-store/)
- [Graph database](https://www.oracle.com/in/autonomous-database/what-is-graph-database/)
- [Multi-model database](https://phoenixnap.com/kb/multi-model-database)