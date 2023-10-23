
![[Pasted image 20231023140737.png]]

[[Transmission Control Protocol/Internet Protocol]] stack has 7 layers

The [[Middleware]] protocol provides common services and protocols that can be used by many different applications:

- Rich set of communication protocols
- (Un)marshalling of data that's necessary for integrated systems
- Naming protocols allow easy sharing of resources
- Security protocols for secure communication
- Scaling mechanisms (e.g. replication & caching)

Layered protocol adapted with middleware protocol:

![[Pasted image 20231023141429.png]]

Types of communication:

- Asynchronous - client sends a request to the server for the client to do something else then check to see a reply from the server
- Synchronous - the client must wait for the server to receive & respond to the request
- Transient - server discards the message when it can't be delivered at the next server or at the receiver
- Persistent - a message is stored at the server as long as it takes to deliver it

Client/Server computing is generally based on 