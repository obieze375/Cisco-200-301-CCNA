# Broadcast Domains

A broadcast domain is the set of devices to which that a broadcast is delivered.

A LAN consists of all devices in the same broadcast domain.

### Summary

* Routers do not forward Ethernet broadcast frames, because the IP routing logic essentially separates broadcast domains. 
* Switches and Hubs forward broadcasts, they use the same logic, flooding LAN broadcasts. 
* Broadcasts sent by a device in one broadcast domain are not forwarded to devices in another broadcast domain. They are typically isolated by each other by a router. 
* VLANs \(Virtual LANs\) are an efficient way of separating broadcast domains. 
* Sizing of broadcast domains are a crucial part of designing VLAN topology, in perfect conditions it should neither be too small or too large.

### Why large broadcast domains are bad

Whenever X amount of hosts send a broadcast ALL hosts receive it. Every device's CPU will then need to process the received frame. In a very large broadcast domain this processing becomes exponential and causes unnessecary interruptions of each device's CPU.









