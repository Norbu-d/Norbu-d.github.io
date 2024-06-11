---
Title: DBM101 Flipped Class 3
categories: [DBS101, Flipped_Class]
tags: [DBS101]
---

### Topic : Set operations in sql and null values in sql

## Set Operations in SQL:

SQL supports set operations to work with multiple sets of data. These operations include:

UNION: This operation combines the results of two or more SELECT queries into a single result set. It removes duplicates by default.

UNION ALL: Similar to UNION, but it includes all rows from all SELECT statements, even if they are duplicates.

INTERSECT: This operation returns only the rows that appear in both result sets of two SELECT statements.

EXCEPT or MINUS: This operation returns only the rows that appear in the first result set but not in the second result set.

Set operations are useful in scenarios where you need to combine or compare data from multiple sources or conditions. They are often used in reporting, data analysis, and when dealing with data from different sources or tables.

<!-- ![alt text](/set-operators-in-sql.png) -->

## NULL Value in SQL:

In SQL, NULL represents a missing or unknown value. It's not the same as zero or an empty string; it signifies the absence of a value or the value is undefined.

Here are some key points about NULL values in SQL:

Handling NULLs: SQL provides functions and operators to handle NULL values, such as IS NULL, IS NOT NULL, COALESCE, and NULLIF.

Arithmetic with NULLs: If any operand in an arithmetic operation is NULL, the result is also NULL.

Aggregations and NULLs: Most aggregate functions ignore NULL values. For example, if you calculate the average of a column containing NULL values, the NULL values will be excluded from the calculation.

Comparison with NULL: Comparing a value with NULL using standard comparison operators (=, <>, <, >, etc.) results in UNKNOWN, not TRUE or FALSE. You should use IS NULL or IS NOT NULL for NULL comparisons.

NULL in Indexes: Most SQL databases allow NULL values in indexed columns. However, be cautious when using NULLs in indexed columns, as they might affect query performance.

NULL values are essential for representing missing or unknown information in databases. They allow for more flexible data modeling and querying but require careful handling to avoid unexpected results in queries and calculations.

<!-- ![alt text](/null.jpg) -->

In class we discussed about the topics in groups with respectred topics to assigned groups and hence we disscussed and explained within our group and after time was up we then went to other groups which had differnt topics disccusing it altogether and learning the above sql operations and null vlues in sql.

