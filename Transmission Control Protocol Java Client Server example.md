
Client implementation:

```
import java.io.*
import java.net.*
class TCPClient{
	public static void main(String argv[]) throws Exception
	{
		String sentence;
		String modifiedSentence;
		
		BufferedReader inFromUser = new BufferedReader(new InputStreamReader(System.in)); /* Creates client input stream*/
		
		Socket clientSocket = new Socket("hostname", 6789); /*Creates client socket to connect to the server*/
		
		DataOutputStream outToServer outToServer = new DataOutputStream(clientSocket.getOutputStream()); /*Creates server's output stream*/
		
		BufferReader inFromServer = new BufferedReader(new InputStreamReader(clientSocket.getInputStream())); /*Creates server's input stream*/
		
		sentence = inFromUser.readLine();
		
		outToServer.writeBytes(sentence + '\n'); \*Sends the inputline to the server*\
		
		modifiedSentence = inFromServer.readLine(); /*Reads the inputline from the server*/
		
		System.out.println("FROM SERVER: " + modifiedSentence);
		
		clientSocket.close();
	}
}
```

Server implementation:

```
import java.io.*
import java.net.*
class TCPServer{
	public static void main(String argv[]) throws Exception
	{
		String clientSentence;
		String capitalisedSentence;
		
		ServerSocket welcomeSocket = new ServerSocket(6789); /*Creates welcoming socket at port 6789 for clients to connect to*/
		
		while(true){
			
			Socket connectionSocket = welcomeSocket.accept(); /*Waits on welcoming socket for contact by client*/
			
			BufferedReader inFromClient = new BufferedReader(new InputStreamReader(connectionSocket.getInputStream())); /*Creates input stream that's attached to the socket*/
			
			DataOutputStream outToClient = new DataOutputStream(connectionSocket.getOutputStream());
		}
	}
}
```