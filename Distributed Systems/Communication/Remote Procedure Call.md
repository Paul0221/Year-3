
Remote Procedure Call (RPC) - requests are sent through local procedure call (packaged as a message) processed, responded through message and then the result is returned from call

RPC is a well engineered procedure that operates in isolation (black box)

- Client sends a request to the server which processes the request and then sends a reply
- There's a delay to process the request and wait for the reply
- Communication between caller and callee can be hidden using procedure-call mechanism

![[Pasted image 20231023145701.png]]

1. Client procedure calls client stub (proxy)
2. Client stub builds message (martials) and calls the local OS
3. Client's OS sends message to remote OS
4. Remote OS give message to server stub
5. Server stub unpacks parameters (unmartials) and calls the server
6. Server does the work and returns the result to the server stub
7. Server builds message containing the reply (martials) and then calls the local OS
8. Server's OS sends the message to the client OS
9. Client's OS gives the message to the client stub
10. Client stub unpacks the result (unmartials) and returrns the result to the client

[[Marshalling and Unmarshalling]]

