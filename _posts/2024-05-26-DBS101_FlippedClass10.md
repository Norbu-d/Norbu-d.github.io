---
Title: DBS101 Flipped Class 10
categories: [DBS101, Flipped_Class]
tags: [DBS101]
---

### Topic : Transaction Properties, steriliability.

## Transaction Properties

A transaction, on the other hand, is the smallest unit of work in the context of a database management system, which has been put in place to guarantee that integrity and consistency of data. The core properties of transactions are encapsulated by the ACID acronym: The four fundamental tenets of ACID Transient data: The data should be kept as briefly as possible in the transaction and should not be accessible to other processes or users.

It also ensures that a transaction is completed as a single, integrated and without the interference of other transaction. It is ‘all or nothing’ in the sense that if at all a transaction is executed then all of the operations within it must be successful. This helps maximize utilization of the buffer, ensures that no partial updates are written to the database and therefore eliminating inconsistencies.

Durability means that in case of a system failure or shutdown the changes to the carried out in a transaction should remain permanent in the database and remain in the state of the new valid state according to all the set rules including constraints and triggers. Precision is kept intact in this property.

This means that isolation confirms that activities from one transaction cannot be seen by other transactions unless the specific transaction is done. It reduces transaction control so that one transaction does not impact or affect the result of another transaction which is in the process of processing. Isolation is usually achieved through concurrency with the help of various ways such as the use of locks and timestamps.

Durability confirms that once a transaction has been processed and committed, the changes made are stored permanently in the system, and will not be lost if there is a power failure or a system crash. This is mostly done through measures like logging and checkpointing.

## Serializability

A concept in concurrency control, is of importance in checking for the validity of multiple executed transactions. A schedule is defined as acyclic schedule if there exists serial schedule that shall offer similar result in executing those transaction operations without overlapping in which transactions are performed in serial manner.

There are two primary types of serializability:There are two primary types of serializability:

There is a concept known as Conflict Serializability which would guarantee that a schedule could be converted to a serial one by swapping the flow of operations that are not conflicting. Two operations are said to be conflicting if: the first operation is part of a specific transaction, the second operation is part of a different transaction, the two operations work on the same variables, and at least one of the operations is a write operation.

The next view is called Serializability, which is a less restrictive form to make sure the schedule yields the same outcome as a certain serial schedule, while not necessarily exchanging operations. This makes it more flexible than the mode with fixed dates, though it is less easy to arrange and document.

Maintaining serialization requires different concurrency control methods like locking protocols like two-phased locking, timestamp based methods and optimistic techniques. Each of the discussed techniques is beneficial and has its drawbacks concerning multifaceted aspects including complexity, performance, and level of concurrency.

In practice, it is not always easy to achieve high concurrency alongside ensuring that the transactions which execute concurrently are serializable. Businesses require their systems to support high throughputs for transactions while at the same time properly preserving transactional integrity to avoid issues like lost updates, damage reads, and uncommitted reads.

Therefore by following the ACID properties and having serializability, database systems can offer a solid and safe means of performing transactions and to maintain high levels of consistency in spite of concurrent processing. These are basic principles of designing applications aimed at helping organizations manage accurate data.