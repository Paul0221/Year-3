
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

b) The sender sends the mes