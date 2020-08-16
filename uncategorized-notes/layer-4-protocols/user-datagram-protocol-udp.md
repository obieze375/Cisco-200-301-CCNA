# User Datagram Protocol \(UDP\)

### Key concepts

1. UDP is a 'Send it and forget it' protocol
2. No sequencing, no acknowledgements
3. No... anything, except for Port numbers and Checksum.

### Usage

UDP is commonly used in online gaming, streaming content such as videos and VOIP calls.

### Constraints

Since the UDP protocol in itself does not do any control measures like TCP to make sure a transmission over the network was successful, application developers have to program applications to explicitly handle the situations that can arise with UDP, like loss of data or no reply at all.





