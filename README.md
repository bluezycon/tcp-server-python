Python TCP Server
=============

1. This TCP server receives incoming requests and echos system information them back to the sender. It starts by creating a TCP/IP socket

1. Then **bind()** is used to associate the socket with the server address. In this case, the address is localhost, referring to the current server, and the port number is 10000

1. Calling **listen()** puts the socket into server mode, and **accept()** waits for an incoming connection.

1. **accept()** returns an open connection between the server and client, along with the address of the client. The connection is actually a different socket on another port (assigned by the kernel). Data is read from the connection with **recv()** and transmitted with **sendall()**

1. The client program sets up its socket differently from the way a server does. Instead of binding to a port and listening, it uses **connect()** to attach the socket directly to the remote address.

1. After the connection is established, data can be sent through the socket with **sendall()** and received with **recv()**, just as in the server.

1. After the connection is established, data can be sent through the socket with **sendall()** and received with **recv()**, just as in the server.

## Project by
* Abhishek Shaji