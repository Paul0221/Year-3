
Peer-to-Peer architectures - processes are all equal as the functions that need to be carried out are represented by every process

Each process acts as a client and a server at the same time

Structured Peer-to-Peer architecture

![[Pasted image 20231019164116.png]]

- Nodes (processes) are organised in an overlay that adheres to a specific, deterministic topology used to look up data
- Makes use of a semantic-free index where each data item is uniquely associated with a key, in turn use an index
	- Common practice is to use a hash function: key(data item) = hash(data item's value)
- Responsible for storing (key, value) pairs