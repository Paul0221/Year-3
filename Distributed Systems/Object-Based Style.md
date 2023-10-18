
![[Pasted image 20231018130709.png]]

Components are objects connected to each other through procedure calls

Objects may be placed on different machines and calls can thus execute across a network (

	e.g. Remote Method Invocation aka RMI

Objects encapsulate data and offer methods on that data without revealing the internal implementation

![[Pasted image 20231018130919.png]]

	Common organisation of a remote object with client-side proxy

Proxy is on the client-side which invokes a method on the object in the server machine

Skeleton is on the server-side which invokes a method on the object in the client machine

Both the proxy and skeleton martial and unmartial an RPC (Remote Procedure Call)

