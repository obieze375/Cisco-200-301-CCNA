# TCP/IP and OSI models

![](../.gitbook/assets/image%20%288%29.png)

![](../.gitbook/assets/image%20%289%29.png)

The OSI model is the preferred reference model for describing network communications.  
The TCP/IP protocol is the preferred protocol stack in most networks today.

There exists a OSI protocol but it failed to become widely adopted at the early inception when TCP/IP had already been established. This is why the use of TCP/IP has now become standard.

![](../.gitbook/assets/image%20%2817%29.png)

### 7 - Application Layer

* The visual representation of the data displayed to the end-user.
* The data processing that is done by an application like a web browser resides in the application layer.

### 6 - Presentation Layer

### 5 - Session Layer

### 4 - Transport Layer

Segment: a chunk of data, with a transport layer header.

![TCP Segment Header](../.gitbook/assets/image%20%2820%29.png)

### 3 - Network Layer

Packet, a chunk of data, with a network layer header.  
Packets are encapsulated in a frame. 

Think about it like the mail inside an envelope. When the packet travels across routers, the addressing is changed on the envelope \(frame\) and passed further along the network until it reaches its destination.

![](../.gitbook/assets/image%20%2825%29.png)

### 2 - Data Link Layer

![](../.gitbook/assets/image%20%2813%29.png)

Frame, a chunk of data, with a Data Link Layer header. The frame encapsulates the packet which contains a segment that contains the payload.

The data link layer is responsible communication, i.e. passing frames within the local network only.

### 1 - Physical Layer

At the physical layer the information is transferred by means of electrical signals, over a medium like copper or fiber.

![](../.gitbook/assets/2020-08-02_13-20-07.gif)





