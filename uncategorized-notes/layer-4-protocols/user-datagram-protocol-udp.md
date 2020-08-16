# User Datagram Protocol \(UDP\)

### Key concepts

1. UDP is a 'Send it and forget it' protocol
2. No sequencing, no acknowledgements
3. No... anything, except for Port numbers and Checksum.

### Usage

UDP is commonly used in online gaming, streaming content such as videos and VOIP calls.

### Constraints

Since the UDP protocol in itself does not do any control measures like TCP to make sure a transmission over the network was successful, application developers have to program applications to explicitly handle the situations that can arise with UDP, like loss of data or no reply at all.

## Vulnerabilities

#### A UDP amplification vulnerability occurs when a UDP service responds with more data or packets than the initial request that elicited the response\(s\)

{% embed url="https://blog.rapid7.com/2016/10/31/understanding-udp-amplification-vulnerabilities-through-rapid7-research/\#:~:text=A%20UDP%20amplification%20vulnerability%20occurs,elicited%20the%20response\(s\).&text=US%2DCERT%27s%20alert%20on%20UDP%2DBased%20Amplification%20Attacks" %}







