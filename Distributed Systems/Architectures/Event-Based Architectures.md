
Event-Based Architectures view distributed systems as a collection of autonomously operating processes

Coordination encompasses the communication and cooperation between processes

Types of coordination:

- Mailbox coordination - doesn't need 2 communicating processes to be executing at the same time for communication to take place
- Event-Based Coordination - process publishes a notification describing the occurrence of an event
![[Pasted image 20231019160207.png]]
	- Other processes may subscribe to a specific kind of notification
- Shared Data-Space - processes communicate through tuples among all the components
![[Pasted image 20231019160529.png]]
	- Tuples - data records consisting of a number of fields similar to a row in a database
