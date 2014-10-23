#Cube
An experiment big data storage system for online service.

##Language
golang

##Basic Plan

### version 0.1
- A abstract key-value storage engine.
- Multi key-value storage libraries, eg; BerkeleyDB, LevelDB
- Performace tests and comparison

### version 0.2
- A data model based on the key-value storage engine.
  - NameSpace
  - Table
  - Region
  - Entry Group
  - Row
  - Locality Group
  - Column
  - Data. Data type: int32/uint32/int64/uint64/float/double/string/protobuf, ,..

### version 0.3
- A consistent replica set using paxos (raft) consensus algorithm.

### version 0.4
- RPC interfaces
- A Master-Worker distributed architecture for this system.

##Features

###High Priority
- Support multi storage media: hdd, ssd, memory.
- Support a cluster across multi datacenters.
- Support multi-tenant. A nameSpace has quota of Table num, Region num, data Amount, and so on. 
  A Table has quota of read/write request num. 

###Low Priority
- Security, Acl and Audit.
- A web monitor.

###References
- Google bigtable http://research.google.com/archive/bigtable-osdi06.pdf
- Google MegaStore http://research.google.com/pubs/archive/36971.pdf
