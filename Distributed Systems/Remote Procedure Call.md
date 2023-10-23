
Remote Procedure Call (RPC) - requests are sent through local procedure call (packaged as a message) processed, responded through message and then the result is returned from call

RPC is a well engineered procedure that operates in isolation (black box)

- Client sends a request to the server which processes the request and then sends a reply
- There's a delay to process the request and wait for the reply
- Communication between caller and callee can be hidden using procedure-call mechanism

![[Pasted image 20231023145701.png]]

- Client procedure calls client stub (proxy)
- Client stub builds message (martials) and calls the local OS
- Client's OS sends message to remote OS
- Remote OS give message to server stub
- Server stub unpacks parameters **