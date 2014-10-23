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
- A data model based on the key-value storage engine. NameSpace -> Table -> Region -> Entry

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
