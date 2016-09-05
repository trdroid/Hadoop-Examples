# HDFS

**Key Features of HDFS**

* Scalability and Availability, achieved by
  - **data replication** - files in HDFS are replicated for a pre-configured number of times 
  - **fault tolerance** - HDFS is built to be tolerant to failures in both software and hardware; in case of a failure the data blocks on the failed nodes are re-replicated
* Optimized for high throughput (works best when reading and writing files of gigabyte sizes and higher), achieved by
  - large block sizes
* Data locality optimizations to reduce network I/O

**HDFS Features added in Hadoop version 2**

* Federation
* High Availability (HA)
