
Client implementation:

```
import java.io.*
import java.net.*

class UDPClient{
	public static void main(String args[]) throws Exception
	{
		BufferedReader inFromUser = new BufferedReader(new InputStreamReader(System.in)); /*Creates the client's input stream*/
		
		DatagramSocket clientSocket = new DatagramSocket(); /*Creates the client socket*/
		
		InetAddress IPAddress = InetAddress.getByName("hostname"); /*Translates hostname to IP address using DNS (Domain Name System)*/
		
		byte[] sendData = new byte[1024];
		byte[] receiveData = new byte[1024];
		
		String sentence = inFromUser.readLine();
		
		sendData = sentence.getBytes();
		
		DatagramPacket sendPacket = new DatagramPacket(sendData, sendData.length, IPAddress, 9876); /*Creates a datagram with data-to-send, length, IP address and port number*/
		
		clientSocket.send(sendPacket); /*Sends the datagram to the server*/
		
		DatagramPacket receivePacket = new DatagramPacket(receiveData, receiveData.length);
		
		clientSocket.receive(receivePacket); /*Reads the datagram from the server*/
		
		String modifiedSentence = new String(receivePacket.getData());
		
		System.out.println("FROM SERVER:" + modifiedSentence);
		
		clientSocket.close();
	}
}
```

Server implementation:

```
import java.io.*
import java.net.*

class UDPServer{
	public static void main(String args[]) throws Exception
	{
		DatagramSocket serverSocket
	}
}
```