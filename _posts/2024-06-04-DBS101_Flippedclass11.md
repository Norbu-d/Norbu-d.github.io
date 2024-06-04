---
Title: DBM101 Flipped Class 11
categories: [DBS101, Flipped_Class]
tags: [DBS101]
---

### Topic : concurrency control,two phase locking,time stamp concurrency control,lock and lactus

## Concurrency control

There are many important techniques in concurrent control such as two-phase locking (2PL), timestamp concurrency control, and the use of lock and latches, which are vital for the management of databases. These mechanisms are used to coordinate the execution of two activities at the same time so that there is no infringement of integrity constraints all over the system. Here's how they fit into the broader context of concurrency control:Here's how they fit into the broader context of concurrency control:

Database Management Systems (DBMS)

Another point, which is fundamental to any DBMS, is dealing with multiple transactions simultaneously. A transaction may be described as a single, programmatic operation that fulfills a specific need in an application by reading, writing, modifying or purging information from a database. Concurrency control therefore aims to enable these transactions to run through their operations as they work on the databases independently without considering the other ongoing transactions as the transactions operate under ACID principles which include Atomicity, Consistency, Isolation, and Durability.

Concurrency control mechanisms are methods which identify; regulate and resolve the conflicts that may arise during concurrent processing of data by several users.


## Two-Phase Locking (2PL)

Two-phase locking is a concurrency control protocol that prevents transaction conflicts by dividing the transaction execution into two phases: In furtherance of a life cycle model, growth and decay can also be noted such as the GROWTH phase and the SHRINKAGE phase. In this particular phase, a transaction obtains the necessary locks in the system; nonetheless, no locks are released. When all the required locks are successfully acquired, the transaction proceeds on the shrink phase of the transaction, in this phase the locks are released one after the other as they were acquired. This protocol ensures that if a transaction gets halfway through a task, then either it concludes successfully or doesn’t stop other transactions from going through.

Advantages:

The concept is quite easy to apply and the user can easily comprehend.

Does not allow for the development of deadlocks if effectively implemented and managed.

Disadvantages:

High contention can occur when multiple transactions need the same resource in the system.

May lead to long waiting times especially where entities are holding locks.

## Timestamp Concurrency Control

Work in progress Timestamp concurrency control employs the application of timestamps to sort transactions and solve for conflict. Every transaction is provided with certain timestamp as its execution begins. Web transactions take place according to increasing order by their timestamps. When a conflict is detected (for instance, two transactions attempt to change the data item concurrently), the transaction with the older timestamp is rolled back and is assigned with a new timestamp whenever it is restarted.

Advantages:

I Hope this is helpful in describing the characteristics of both K-V stores and Hash tables: K-V stores are much more efficient for read-heavy workloads because write operations are rare.

Simplifies conflict resolution.

Disadvantages:

It is not suitable to use where the transactional, duration and severity can have different values.

If a transaction receives newer timestamps and cannot end within a finite amount of time, it will starve.

## Locks and Latches

Locks and latches are methodologies that are applied for regulating the degree of concurrency, achieved by protection of presented shared assets against simultaneous access.

DBMS has locks that help to avoid concurrency control problems such as two transactions using the same resource at once. Locks can be categorized as well, with shared locks being able to allow read access to a shared resource while exclusive locks prevent any access to the shared resource by other processes. In most cases, locks can be built on rows, pages, as well as entire tables, based on the workload’s level of specificity.

Latches are similar to locks but operate on a single, transactional level to ensure that data structures within the database engine are not simultaneously corrupted or modified by multiple transactions. It is conventionally utilized to guarding internal data structures against concurrent alteration, in order to maintain the integrity of the information and minimize the risk of race condition.

## summary 

Locks and latches are önemli for dealing with concurrency issues in database systems. The difference between locks and latches is quite simple: while the use of locks helps to regulate access to data to the outside world, latches are crucial for internal purposes to protect consistency and adequate rates of performance.

To sum up, concurrency control is an essential and core property of database management systems responsible for preserving the data’s integrity and consistency in the case of multiple concurrent activity. Two-phase locking and checking the timestamp are other strategies that address the problem of conflicting transactions which also have their pros and cons. To understand the uses of locks and latches as factors that implement these controls, it is crucial to learn the design of effective and robust database systems.

