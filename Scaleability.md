#distributed-systems #fundamentals  #flashcards/fundamentals 

How to scale a database?
?
If you're working with a **relational database** that already contains a large amount of data, one common approach is to use **master-slave replication**. This allows read operations to be distributed across replicas, improving read performance and availability. However, writes still go to the master, so this approach doesn't scale writes.

If you're starting a new project and scalability is a key concern, consider using a **NoSQL database** like **MongoDB**, which supports **sharding** natively. Sharding distributes data across multiple nodes, allowing both reads and writes to scale horizontally.

If you **must use a relational database** for a new system — or if the amount of data to migrate is still manageable — you can design your schema to better support scaling. One strategy is to **denormalize the data** to reduce or eliminate the need for joins, which are problematic in a sharded setup. In a **sharded relational database**, data is split across multiple physical nodes (shards). Performing joins across shards is slow and complex, which can hurt performance and negate the benefits of sharding.
+++

What is a sharding node?
?
A **sharding node** (or **shard node**) is a **physical or virtual machine** that hosts a **database instance containing a subset of the overall dataset** in a **sharded database system**.

In a sharded architecture:

- The full dataset is split into **shards** based on a **shard key** (e.g., user ID, region).
- Each **shard** is stored on a separate **sharding node**.
- A **shard node** runs its own independent **database instance** (e.g., MongoDB, PostgreSQL).
- These nodes collectively form the complete database, but **each node only stores part of the data**.
+++