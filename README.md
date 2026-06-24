
# MiniRDBMS

**MiniRDBMS** is a modular relational database engine developed in **C++** that implements the fundamental components of modern database management systems. The project provides a hands-on exploration of database internals, including storage management, buffer management, schema catalogs, record organization, and B+ Tree indexing.

Designed as an educational yet architecturally structured system, MiniRDBMS demonstrates how relational databases store, retrieve, cache, and index data through a layered architecture inspired by production-grade DBMS implementations.

---

## Highlights

* Relational table and schema management
* Block-based storage architecture
* Buffer pool management for efficient disk access
* Relation and attribute catalog management
* Record insertion, deletion, update, and retrieval
* B+ Tree indexing for optimized search operations
* Metadata caching for improved performance
* Layered and modular DBMS architecture
* Educational implementation of database storage and indexing mechanisms

---

## Architecture Overview

MiniRDBMS is organized into independent layers, each responsible for a specific aspect of database functionality.

```text
Frontend Interface
        │
        ▼
Algebra Layer
        │
        ▼
Schema Layer
        │
        ▼
Block Access Layer
        │
        ▼
Cache Layer
        │
        ▼
Buffer Layer
        │
        ▼
Disk Layer
```

### Core Components

#### Disk Manager

Handles persistent storage and block-level disk operations.

#### Buffer Manager

Manages in-memory buffering of disk blocks to reduce I/O overhead and improve access performance.

#### Relation & Attribute Cache

Maintains metadata caches for efficient schema and relation lookup.

#### Schema Manager

Responsible for relation catalogs, attribute catalogs, and schema definitions.

#### Block Access Layer

Provides abstraction for reading and writing records from storage blocks.

#### B+ Tree Index Manager

Implements balanced tree indexing to support efficient record search and retrieval.

#### Query Processing Layer

Executes relational operations and coordinates interactions between higher-level components and storage layers.

---

## Technical Concepts Demonstrated

* Database Storage Engines
* Buffer Pool Management
* Metadata Catalogs
* Record Management
* B+ Tree Indexing
* Block-Oriented Storage
* Relation Caching
* Query Processing Fundamentals
* Layered System Design
* File-Based Persistence

---

## Technology Stack

* **Language:** C++
* **Architecture:** Layered Modular Design
* **Data Structures:** B+ Trees, Catalog Tables, Buffer Pools
* **Storage:** Block-Based File Storage

---

## Why This Project?

Modern relational databases such as PostgreSQL, MySQL, and Oracle rely on sophisticated storage engines, caching mechanisms, indexing structures, and metadata management systems. MiniRDBMS was built to bridge the gap between theoretical DBMS concepts and practical implementation by recreating these core components in a simplified yet realistic environment.

The project serves as a foundation for understanding how database systems manage data efficiently and how internal components interact to provide reliable storage and retrieval operations.

---

## Future Enhancements

* SQL Parser
* Query Optimizer
* Transaction Management
* Concurrency Control
* Crash Recovery & Logging
* Cost-Based Query Planning
* User Authentication & Authorization
* Distributed Storage Support

---

