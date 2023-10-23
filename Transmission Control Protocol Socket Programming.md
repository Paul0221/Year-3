
Transmission Control Protocol application provides reliable, in-order transfer of bytes between client and server

Stages of Transmission Control Protocol Socket programming:

1) Server process must first be running and must have created a socket to welcome a client's contact
2) The client contacts the server by creating a client-local TCP socket which specifies the IP address and port number of server process 
3) When the client creates the socket the client TCP establishes connection to the server TCP
4) When contacted by the client, the server TCP creates a new socket for server processes to communicate with the client which allows server to talk to multiple clients
	- Source port numbers are used to distinguish clients


Client-server app example:

![[Pasted image 20231024000444.png]] 

1) Client reads the line from the client's standard input stream (inFromUser) and sends it to the server via output stream (outToServer)
2) The server reads the line from the socket
3) The server converts the line to uppercase and then sends it back to the client
4) The client reads and then prints the modified line from the server's input stream (inFromServer)

TCP client/server socket interaction:

![[Pasted image 20231024001136.png]]

- ServerSocket(int port) - used to listen for connections on a specified port number
- accept() - used to liste