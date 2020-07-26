Socket Programming 


The goal of Socket Programming is to build client/server applications which communicate 
using sockets.

A socket is one endpoint of a two-way communication link between two programs running on the network.
A socket is bound to a port number so that the Transport (TCP) layer can identify the application that data
is destined to be sent to. An endpoint is a combination of an IP address and a port number.

A socket is an interface between the transport and application layer within a host.
It is also referred to as API (Application Programming Interface). When creating a network application, 
a developer has to write the code for both clients and server programs.


2 Socket Types 

1) UDP (unreliable, connectionless datagram)

2) TCP (reliable, byte stream oriented, connection oriented)


Socket Programming with UDP 

- no connection between client and server 

- no handshake before sending data 

- sender program explicitly attaches the IP destination address and port number to the packets

- receiver program extracts the sender's IP address and port number from the received packet

- data may be lost or out of order


Socket Programming with TCP 

- the client must connect to the server 

- the server process must first be running 

- the server must have created a socket (door) that welcomes the client's contact 

- the client connects to the server by creating a TCP socket and establishing a connection to the server 
using the IP and port of the server 

- the server creates a new socket for the server process to communicate with a particular client that 
connects with it 

- this allows the server to communicate with multiple clients 

- source port numbers are used to distinguish clients 


** Look into Python socket programming, and the Python P2P filesharing app example