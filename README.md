# fp-rocks
A NashFP playground where we use RocksDB from various FP languages

## What is RocksDB?

From [Wikipedia](https://en.wikipedia.org/wiki/RocksDB)...

> RocksDB is a high performance embedded database for key-value data. It is a fork of LevelDB by Facebook optimized to exploit many central processing unit (CPU) cores, and make efficient use of fast storage, such as solid-state drives (SSD), for input/output (I/O) bound workloads. It is based on a log-structured merge-tree (LSM tree) data structure. It is written in C++ and provides official application programming interface (API) language bindings for C++, C, and Java; alongside many third-party language bindings.
> ...
> RocksDB, like LevelDB, stores keys and values in arbitrary byte arrays, and data is sorted byte-wise by key or by providing a custom comparator.
>
> RocksDB provides all of the features of LevelDB, plus:
> Transactions
> Backups[16] and snapshots
> Column families
> Bloom filters
> Time to live (TTL) support
> Universal compaction
> Merge operators
> Statistics collection
> Geospatial indexing
> 
> RocksDB is not an SQL database (although MyRocks combines RocksDB with MySQL). Like other NoSQL and dbm stores, it has no relational data model, and it does not support SQL queries. Also, it has no direct support for secondary indexes, however a user may build their own internally using Column Families or externally. Applications use RocksDB as a library, as it does not provide a server or command-line interface.


### Official website

From the official website at [https://rocksdb.org/](https://rocksdb.org/)...

> **High Performance**:
> RocksDB uses a log structured database engine, written entirely in C++, for maximum performance. Keys and values are just arbitrarily-sized byte streams.

> **Optimized for Fast Storage**: 
> RocksDB is optimized for fast, low latency storage such as flash drives and high-speed disk drives. RocksDB exploits the full potential of high read/write rates offered by flash or RAM.

> **Adaptable**: 
> RocksDB is adaptable to different workloads. From database storage engines such as MyRocks to application data caching to embedded workloads, RocksDB can be used for a variety of data needs.

> **Basic and Advanced Database Operations**: 
> RocksDB provides basic operations such as opening and closing a database, reading and writing to more advanced operations such as merging and compaction filters.


## Ideas

* Create an Elixir (or Erlang) project that lazily persists ETS tables to disk (similar to [persistent_ets](https://github.com/michalmuskala/persistent_ets)), but use RocksDB as the backing store.
* ... more ideas please ....


## How to play along
Join the fun! Add a directory to this repo containing your code.

By convention, we use directory names that tell who wrote the code and what language it's in, separated by a `+`. For example: `bryan_hunter+elixir`.

If you don't have a clue where to start take a peek at some of the existing solutions. 

If you don't already have the right permissions to push to this repo, file an issue! We'll hook you up. You can also submit a pull request for your contributions. However you like to roll.
