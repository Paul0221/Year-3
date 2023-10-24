
User Datagram Protocol has no connection between the client and server which provides unreliable transfer of datagrams between client and server

- No handshaking
- Sender explicitly attaches IP address and port of destination to each packet
- Server must extract an IP address and port of sender from the received packet
- Transmitted data maybe received out of order or lost

UDP client/server socket interaction:

![[Pasted image 20231024010331.png]]

Client-server app example:

