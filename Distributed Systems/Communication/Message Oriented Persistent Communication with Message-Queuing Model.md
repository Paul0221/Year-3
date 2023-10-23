
Message Oriented Persistent Communication with Message-Queuing Model - asynchronous persistent communication through support of middleware-level queues

Queues correspond to buffers at communication servers

Message Oriented Persistent Communication with Message-Queuing primitives:

- Put - append a message to a specified queue
- Get - block until the specified queue is nonempty and remove the first message
- Pull - check a specified queue for messages and remove the first (never block)
- Notify - install a handler to be called when a message is put into the specified queue

Basic interface to queue in a message-queuing system:

![[Pasted image 20231023230325.png]]

a) The sender sends the message and the receiver receives the message as both are running

b) The sender sends the message but the receiver doesn't receive the message yet as it's not running

c) The sender already sent a message and is now doing other things but now the receiver is running and can receive the message

d) The sender already sent a message and is now doing other things but the receiver hasn't received the message as it's not running

General architecture of a message-queuing system:

![[Pasted image 20231023230728.png]]

- Shows the relationship between queue-level addressing & network-level addressing

General organisation of a message-queuing system with a network of routers:

![[Pasted image 20231023230904.png]]

An example of message-queuing with a network of routers is [[Advanced Message Queueing Protocol]]

