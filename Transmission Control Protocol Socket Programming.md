
Transmission Control Protocol application provides reliable, in-order transfer of bytes between client and server

Stages of Transmission Control Protocol Socket programming:

- Server process must first be running and must have created a socket to welcome a client's contact
- The client contacts the server by creating a client-local TCP socket which specifies the IP address and port number of server process
- When the client creates the socket the client TCP establishes connection to the server TCP
- When contacted by the client, the server TCP creates a new socket for server processes to communicate with the client which allows server to talk to multiple clients
	- Source port numbers are used to distinguish clients


Client-server app example: