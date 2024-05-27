---
Title: DBS101 Flipped Class 9
categories: [DBS101, Flipped_Class]
tags: [DBS101]
---

### Topic : Advanced Topics in Query Optimization, Materilized views.

### Advanced Topics in Query Optimization

Abstract: In this paper we considered some advanced topics related to query optimization including query classification and modeling, query transformation techniques, query optimization methods based on artificial intelligence and inductive databases.

Query optimization is yet another critical component of database management systems with a specific aim at improving the efficiency of query processors. There are additional aspects in this area to refine the query performance further, which involves more specialized approaches to diminish the computational load in the system. One important paradigm is the cost-based optimization, where instead of choosing a fixed order of table access and joining, multiple possibilities are estimated and the one with lowest overall cost selected based on factors such as necessary I/O operations, CPU requirements, or network latency. Adaptive Query Processing AQP is another smart technique that enables the system to modify the method of query execution regarding feedback given during the runtime and variation in data.

Another important sub-field is parallel query processing in which the tasks are divided into subtasks of the query and processed with more than one processor or computer system to gain a better and faster result. Further, their integration to query optimizer has slowly started to emerge in the recent past. One of the biggest advantages of machine learning is that based on the history of queries it becomes a lot easier and wiser to make certain optimization decisions on the best execution plans to employ. Also, in the query optimization, materialized views enable the pre-computation and storage of results, and will then be used to respond to additional similar queries relatively fast.

### Materialized Views

Materialized views are a valuable function in databases which is often an outcome of a query stored in physical format so as to get better result as early as possible of complicated queries. In contrast to the standard views which are actually created only when the data is accessed and until then exist only as a concept, the materialized views can offer notable performance improvements because they avoid the need to re-run certain operations. It is most useful when applied in data warehousing and business intelligence architectures in which computational complexity is frequently performed in query execution.

Some information that needs to be updated frequently may require the use of materialized views for constant updating, making it an important feature for the database. Some approaches are mentioned below: Incremental view maintenance (IVM) only updates the materialized view for those changes since the last time it was refreshed or rewritten, saving time and energy as compared to rewinding the entire view. In addition, it is also possible to create indexes and partitions for materialized views to gain better access and processing times as well as control large data volumes.

Selecting materialized views has some dependency on storage overheads and the quarries that implement it gives better performance. It is also possible to enlist the help of further algorithms and heuristics that enable one to choose the ideal set that will be materialized with regard to these aspects so that performance will be optimized. For those of you who are working as DBAs and IT architects, the importance of MVs remains crucial to deal with the challenges of modern growing databases.

It therefore becomes clear that organizations can greatly improve their database and query performance through the optimization inherent in popular query optimization techniques as well as properly optimizing the use of materialized views.