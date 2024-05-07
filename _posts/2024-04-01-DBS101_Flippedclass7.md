---
Title: DBM101 Flipped Class 7
categories: [DBS101, Flipped_Class]
tags: [DBS101]
---

### Topic : Disk Block Implementation,  Redundant Array of Independent Disks,  Buffer Pool Management, chidb:Building a Simple Relational Database System from Scratch, How to build a relational database from scratch.
---

## Disk Block Implementation

Disk Block Implementation defines how files and directories are stored, how disk space is managed, and how to make everything work efficiently and reliably.

Block is the smallest unit of data storage. It is used to read a file or write data to a file. Block is also a sequence of bits and bytes. A sector is a physical spot on a formatted disk that holds information.

each file occupies a contiguous set of blocks on the disk. For example, if a file requires n blocks and is given a block b as the starting location, then the blocks assigned to the file will be: b, b+1, b+2,…… b+n-1.

Disk space should be allocated to files such that the disk space is utilized effectively and files can be accessed quickly. There are three different methods of allocation: Contiguous allocation, Linked allocation and Indexed allocation.

