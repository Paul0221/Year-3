
Resource-Based Architectures views a distributed system as a collection of resources individually managed by components

Resources may be added, removed, retrieved and modified by (remote) applications

- Resources are identified through a single naming scheme (every resource has a logical name)
- All services offer the same interface
- Messages sent to/from a service are fully self-described
- After executing an operation at a service, that component forgets everything about the caller (stateless as oppose to stateful)

Resource-Based Architectures adopt Representational State Transfer (REST) web services following the basic CRUD operations:

- Create a new resource (POST operation)
- Retrieve the state of a resource in some representation (GET operation)
- Update a resource by transferring new state (PUT operation)
- Delete a resource (DELETE operation)

Types of operations carried out by sending HTTP requests:

- Create a bucket/object with POST along with URL
- Listing objects with GET on a bucket name
- Reading an object with get on a full URL