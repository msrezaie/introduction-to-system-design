# Databases and Caching

## Overview

This lesson focuses on understanding the basics of databases, how to choose one, and the concepts of normalization and denormalization. It will also delve into indexing and ACID databases, as well as caching for performance enhancement.

## Learning Objectives

- Understand SQL vs NoSQL
- Learn about normalization and denormalization
- Understand ACID databases
- Learn about caching techniques and tools

## Topics Covered

- Choosing a database
- SQL vs NoSQL
- Denormalization
- Normalization
- Indexing
- ACID Databases
- Caching for performance
- Redis, memcache, cdn caching


## Part 1 - Database

Databases are structured collections of data, used to store and manipulate information. They are essential for designing systems that handle large volumes of data efficiently. Databases allow for data retrieval, modification, and deletion using structured query language (SQL). They support ACID properties: Atomicity, Consistency, Isolation, Durability, ensuring reliable transactions.

Databases can be broadly categorized into relational databases (e.g., PostgreSQL, MySQL) and non-relational databases (e.g., MongoDB, Cassandra). Relational databases use tables to store data and SQL for queries. Non-relational databases, also known as NoSQL databases, store data in various formats like documents, key-value pairs, and graphs.

### 1. SQL vs NoSQL
What’s SQL, https://aws.amazon.com/what-is/sql/

What’s  NoSQL, https://www.mongodb.com/nosql-explained

Which one is better to use, https://www.geeksforgeeks.org/sql/sql-vs-nosql-which-one-is-better-to-use/

### 2. Normalization & Denormalization
**Normalization**: Database normalization is a process used to organize a database into tables and columns.

Three reasons to normalize a database:
1. Minimize duplicate data,
2. Minimize or avoid data modification issues
3. Simplify queries.

Database Normalization Explained in Simple English, https://www.essentialsql.com/database-normalization/

**Denormalization**: Denormalization is a database optimization technique where redundant data is intentionally added to one or more tables to reduce the need for complex joins and improve query performance.

When to Denormalize Guide, https://www.datacamp.com/tutorial/denormalization

### 3. Indexing
Indexing is a technique used in databases to speed up data retrieval operations. It creates pointers to data in tables, significantly reducing the time taken for query responses. While indexing speeds up reads, it can slow down writes as indexes need updating.

Indexing in database, https://www.geeksforgeeks.org/dbms/indexing-in-databases-set-1/

### 4. ACID & Transactions
**ACID transactions** refer to four properties that ensure the reliable processing of database transactions. The four principles are: Atomicity, Consistency, Isolation, Durability.

Read more,
https://www.geeksforgeeks.org/dbms/acid-properties-in-dbms/
https://www.datacamp.com/blog/acid-transactions

### Resources
Top 10 trade offs in database design, 
https://tradeoffs.dev/article/Top_10_tradeoffs_in_database_design.html

Video Presentations & Talks
1. "SQL vs NoSQL" by Martin Fowler, https://www.youtube.com/watch?v=qI_g07C_Q5I
2. Learn how to design and plan a database for beginners, https://www.youtube.com/watch?v=ztHopE5Wnpc

Interactive Learning
1. SQLBolt (Interactive SQL Tutorial), https://sqlbolt.com/
2. MongoDB University (Free NoSQL Courses), https://university.mongodb.com/
3. DB Fiddle (Online SQL Playground), https://www.db-fiddle.com/

## Part 2 - Caching
**Caching** is a concept that involves storing frequently accessed data in a location that is easily and quickly accessible. The purpose of caching is to improve the performance and efficiency of a system by reducing the amount of time it takes to access frequently accessed data.

Caching is a technique used to store copies of frequently accessed data in a high-speed memory layer so that future requests can be served faster. It helps improve performance and scalability. Common caching strategies include in-memory caching (e.g., Redis, Memcached) and browser caching.

https://www.geeksforgeeks.org/system-design/caching-system-design-concept-for-beginners/

**Redis, memcache and cdn cache**, these are all caching technologies, but they operate at different levels and serve distinct purposes.

https://www.linkedin.com/pulse/caching-layers-explained-cdn-redis-memcached-why-matter-deepak-dalal-i5z0c/

1. ### Redis
    Redis (REmote DIctionary Server) is an open source, in-memory, NoSQL key/value store that is used primarily as an application cache or quick-response database. https://www.ibm.com/think/topics/redis
2. ### Memcached
    Memcached is an open source, in-memory, key-value store. It is used for speeding up dynamic web applications with microseconds latency, making it useful as a cache or session store.
https://www.geeksforgeeks.org/system-design/what-is-memcached/

3. ### Redis vs Memcached Comparison
    Redis and Memcached are two of the most popular choices among developers. Both are designed to accelerate web applications by caching data, thereby reducing the load on databases and improving response times. Redis, known for its rich set of features, supports complex data structures and offers persistence options, making it versatile for various use cases. Memcached, on the other hand, is celebrated for its simplicity, speed, and efficiency in handling large amounts of ephemeral data.
https://www.geeksforgeeks.org/dbms/difference-between-redis-and-memcached/

4. ### CDN & Browser Caching
    CDN, a content delivery network (CDN) is a network of interconnected servers that speeds up webpage loading for data-heavy applications. https://www.geeksforgeeks.org/websites-apps/what-is-cdn/
Browser Caching, https://www.cloudflare.com/learning/cdn/what-is-caching/#:~:text=What%20does%20a%20browser%20cache%20do%3F

5. ### Cache Invalidation
    Cache invalidation is the process of invalidating cache by removing data from a system’s cache when that data is no longer valid or useful. In other words, you’re getting rid of old or outdated cached content that’s stored in the cache. https://redis.io/glossary/cache-invalidation/

### Resources
Video Presentations

&emsp;&emsp;What’s CDN, https://www.youtube.com/watch?v=Bsq5cKkS33I

Performance & Monitoring

&emsp;&emsp;Difference between latency and throughput, https://aws.amazon.com/compare/the-difference-between-throughput-and-latency/

Cache Warming Strategies

&emsp;&emsp;pre-populate caches: https://www.geeksforgeeks.org/system-design/what-is-pre-caching/

Caching Strategies and How to Choose the Right One, 
https://codeahoy.com/2017/08/11/caching-strategies-and-how-to-choose-the-right-one/

Cloudflare CDN Learning Center, 
https://www.cloudflare.com/learning/cdn/what-is-a-cdn/

Google Developers - Http caching, 
https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching

Redis University (Free Courses), 
https://university.redis.io/academy

More on what’s memcached, 
https://aws.amazon.com/elasticache/what-is-memcached/

Memecached Wiki, 
https://docs.memcached.org/
