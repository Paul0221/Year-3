
![[Pasted image 20231023140737.png]]

Transmission Control Protocol/Internet Protocol (TCP/IP) stack has 7 layers

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

Client/Server computing is generally based on transient synchronous communication where:

- Client and server have to be active at the time of communication
- Client issues request and blocks until it receives a reply
- Server waits only for incoming requests and subsequently processes them
- Drawback is that the client and server can't do other things whilst waiting for a request

[[Message Oriented Middleware]] aims at high level persistent asynchronous communication where:

- Processes send each other messages which are queued
- Sender doesn't wait for immediate reply but can do other things
- [[Middleware]] often ensures fault tolerance to make sure message is not lost

Methods of communication:

- [[Message Oriented Communication]]
- [[Message Oriented Persistent]]
- [[Message Passing Interface]]
- [[Remote Method Invocation]]
- [[Remote Procedure Call]]



