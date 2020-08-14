# Layer 4 Protocols

The OSI transport layer \(Layer 4\) is using protocols that perform

* [Connection-oriented communication](https://en.wikipedia.org/wiki/Connection-oriented_communication): It is normally easier for an application to interpret a connection as a [data stream](https://en.wikipedia.org/wiki/Data_stream) rather than having to deal with the underlying connection-less models, such as the [datagram](https://en.wikipedia.org/wiki/Datagram) model of the [User Datagram Protocol](https://en.wikipedia.org/wiki/User_Datagram_Protocol) \(UDP\) and of the [Internet Protocol](https://en.wikipedia.org/wiki/Internet_Protocol) \(IP\). 
* Same order delivery: The network layer doesn't generally guarantee that packets of data will arrive in the same order that they were sent, but often this is a desirable feature. This is usually done through the use of segment numbering, with the receiver passing them to the application in order. This can cause [head-of-line blocking](https://en.wikipedia.org/wiki/Head-of-line_blocking). 
* [Reliability](https://en.wikipedia.org/wiki/Reliability_%28computer_networking%29): Packets may be lost during transport due to [network congestion](https://en.wikipedia.org/wiki/Network_congestion) and errors. By means of an [error detection code](https://en.wikipedia.org/wiki/Error_detection_code), such as a [checksum](https://en.wikipedia.org/wiki/Checksum), the transport protocol may check that the data is not corrupted, and verify correct receipt by sending an [ACK](https://en.wikipedia.org/wiki/Acknowledgement_%28data_networks%29) or [NACK](https://en.wikipedia.org/wiki/Negative-acknowledge_character) message to the sender. [Automatic repeat request](https://en.wikipedia.org/wiki/Automatic_repeat_request) schemes may be used to retransmit lost or corrupted data. 
* [Flow control](https://en.wikipedia.org/wiki/Flow_control_%28data%29): The rate of data transmission between two nodes must sometimes be managed to prevent a fast sender from transmitting more data than can be supported by the receiving [data buffer](https://en.wikipedia.org/wiki/Data_buffer), causing a buffer overrun. This can also be used to improve efficiency by reducing [buffer underrun](https://en.wikipedia.org/wiki/Buffer_underrun). 
* [Congestion avoidance](https://en.wikipedia.org/wiki/Congestion_avoidance): [Congestion control](https://en.wikipedia.org/wiki/Congestion_control) can control traffic entry into a telecommunications network, so as to avoid [congestive collapse](https://en.wikipedia.org/wiki/Congestive_collapse) by attempting to avoid oversubscription of any of the processing or [link](https://en.wikipedia.org/wiki/Data_link) capabilities of the intermediate nodes and networks and taking resource reducing steps, such as reducing the rate of sending [packets](https://en.wikipedia.org/wiki/Packet_%28information_technology%29). For example, [automatic repeat requests](https://en.wikipedia.org/wiki/Automatic_repeat_request) may keep the network in a congested state; this situation can be avoided by adding congestion avoidance to the flow control, including [slow-start](https://en.wikipedia.org/wiki/Slow-start). This keeps the bandwidth consumption at a low level in the beginning of the transmission, or after packet retransmission. 
* [Multiplexing](https://en.wikipedia.org/wiki/Multiplexing): [Ports](https://en.wikipedia.org/wiki/TCP_and_UDP_port) can provide multiple endpoints on a single node. For example, the name on a postal address is a kind of multiplexing, and distinguishes between different recipients of the same location. Computer applications will each listen for information on their own ports, which enables the use of more than one [network service](https://en.wikipedia.org/wiki/Network_service) at the same time. It is part of the transport layer in the [TCP/IP model](https://en.wikipedia.org/wiki/TCP/IP_model), but of the [session layer](https://en.wikipedia.org/wiki/Session_layer) in the OSI model.

{% embed url="https://en.wikipedia.org/wiki/Transport\_layer" caption="Conveniently taken from a great wikipedia page" %}

The protocols mainly used are

* Transmission Control Protocol \(TCP\)
* User Datagram Procol \(UDP\)

### Multiplexing

For multiple applications from the same IP address to communicate with the same protocols at the same time the concept of multiplexing is used to solve the problem.

Multiplexing relies on a concept called a socket. A socket consists of three things:

* An IP address 
* A transport protocol 
* A port number

### Port numbers



* Well Known \(System\) Ports: Numbers from 0 to 1023, assigned by IANA, with a stricter review process to assign new ports than user ports.  
* User \(Registered\) Ports: Numbers from 1024 to 49151, assigned by IANA with a less strict process to assign new ports compared to well-known ports.  
* Ephemeral \(Dynamic, Private\) Ports: Numbers from 49152 to 65535, not assigned and intended to be dynamically allocated and used temporarily for a client application while the app is running.





