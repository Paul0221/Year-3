
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
		
		DatagramPacket sendPacket = new DatagramPacket(sendData, sendData.length)
	}
}
```