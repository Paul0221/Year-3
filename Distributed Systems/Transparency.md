Limited transparency in Distributed Systems as sockets are only directly visible to developers

Significant amount of explicit code need to establish communication between client & server (TCP/IP, UDP/IP)

Types of transparency in Distributed Systems:

- Access - hide differences in data representation & how objects are accessed
- Location - hide object/server location
- Migration - hide object which moves to another server
- Relocation - hide object moving to another location while in use
- Replication - hide replicated object
- Concurrency - hide object shared by several competitive users
- Failure - hide failure & recovery of an object so that if 1 machine object fails, it doesn't impact other machines