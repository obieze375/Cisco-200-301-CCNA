# Collision Domains and Broadcast Domains

## Carrier-sense multiple access with collision detection \(CSMA/CD\) <a id="firstHeading"></a>



### Collision Domain

A collision domain is the set of NICs and device ports for which if they sent a frame at the same time, the frames would collide.

This means each collision domain only can have one sender at a time.

### Hubs

* An Ethernet hub does not forward a traffic like a switch.  
* The hub acts a multiport repeater, blindly regenerating and repeating any electrical signal out all other ports, ignoring CSMA/CD rules. 
* Ethernet hubs use physical layer processing to forward data. 
* A hub does not interpret the incoming signal, it simply repeats the signal and forwards it out of all ports except the incoming port. 
* A switch interprets the signal as a Frame and looks at the source and destination MAC address.

### Bridges

* Bridges were the predecessors of the modern layer 2 switch. A bridge is used to sit between the hub to divide the network collision domains. 
* By doing so, they increase the capacity because it effectively creates a separate instance of CSMA/CD, creating multiple smaller collision domains. 
* Bridges hold Ethernet frames in memory, waiting to send out the outgoing interface based on CSMA/CD rules.  
* In cases where the frame destination resides in the same collision domain the bridge would not need to forward it.

### Switches

LAN switches are functionally similar to bridges but operate at much faster speeds with additional features. Like bridges, switches segment a LAN into separate collision domains, each with its own capacity. Each single link in a modern LAN is considered its own collision domain, even if no collisions can actually occur in that case.









