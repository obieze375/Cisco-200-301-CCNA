# Transmission Control Protocol \(TCP\)

 TCP is [connection-oriented](https://en.wikipedia.org/wiki/Connection-oriented_communication), and a connection between client and server is established before data can be sent. The server must be listening \(passive open\) for connection requests from clients before a connection is established. Three-way handshake \(active open\), [retransmission](https://en.wikipedia.org/wiki/Retransmission_%28data_networks%29), and error-detection adds to reliability but lengthens [latency](https://en.wikipedia.org/wiki/Latency_%28engineering%29). Applications that do not require reliable [data stream](https://en.wikipedia.org/wiki/Data_stream) service may use the [User Datagram Protocol](user-datagram-protocol-udp.md) \(UDP\), which provides a [connectionless](https://en.wikipedia.org/wiki/Connectionless_communication) [datagram](https://en.wikipedia.org/wiki/Datagram) service that prioritizes time over reliability.

{% embed url="https://en.wikipedia.org/wiki/Transmission\_Control\_Protocol" caption="Check out the really good Wikipedia page to review and solidify details." %}

## Three-way handshake

TCP needs to establish a connection in a certain way defined by the protocol before any transmission can be made. The connection establishment process initializes **Sequence** and **Acknowledgement** fields and **Port number** that will be used.

### SYN



## Vulnerabilities

There are vulnerabilities to TCP including [denial of service](https://en.wikipedia.org/wiki/Denial-of-service_attack), [connection hijacking](https://en.wikipedia.org/wiki/TCP_sequence_prediction_attack), TCP veto, and [reset attack](https://en.wikipedia.org/wiki/TCP_reset_attack). For network security, [monitoring](https://en.wikipedia.org/wiki/Network_monitoring), and [debugging](https://en.wikipedia.org/wiki/Debugging_pattern), TCP traffic can be intercepted and logged with a [packet sniffer](https://en.wikipedia.org/wiki/Packet_analyzer).

## 

