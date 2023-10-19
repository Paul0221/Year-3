
Resource-Based Architectures views a distributed system as a collection of resources individually managed by components

Resources may be added, removed, retrieved and modified by (remote) applications

- Resources are identified through a single naming scheme (every resource has a logical name)
- All services offer the same interface
- Messages sent to/from a service are fully self-described
- After executing an operation at a service, that component forgets everything about the caller (state)