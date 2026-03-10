# Assignment 1: Implementing Caching Strategies and Database Indexes

## Objective

Learn to implement basic caching strategies and create indexes to optimize database performance.

## Expected Capabilities

- Understand and implement basic caching
- Create indexes in a database

## Instructions

### Part 1

**Install Redis**

Install Redis server to use as a caching layer.

```
N/A
```

**Setup a Basic Cache with Redis**

Implement a basic cache for storing key-value pairs using Redis.

```
SET mykey 'value'
```

### Part 2

**Create Index on Database**

Create an index on a sample dataset to improve query performance.

```
CREATE INDEX idx_name ON sample_table (column_name);
```

## Tasks

### Task 1: Examine Cache Effectiveness

Access cached data and observe the performance difference.

```
GET mykey
```

### Task 2: Query Indexed Database

Run a query on an indexed and non-indexed database table. Compare the performance.

```
SELECT * FROM sample_table WHERE column_name = 'value';
```

## Submission Instructions

Submit screenshots showing your Redis setup and results of indexed query performance testing.

## Checklist

- [ ] Redis installed
- [ ] Key-value pair set in Redis
- [ ] Index created on database
- [ ] Query performance compared

## Check for Understanding

**How does caching help in system design?**

- Increases storage capacity
- Increases data retrieval speed
- Increases data accuracy

**Answer:** [Your answer here]

**What is the trade-off of using indexing in databases?**

- Faster writes, slower reads
- Faster reads, slower writes
- Slower storage, faster reads

**Answer:** [Your answer here]