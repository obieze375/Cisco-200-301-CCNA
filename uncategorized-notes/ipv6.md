# IPv6

#### What we know about IPv4 can be transferred to IPv6

* Generally inherits the usage and properties of IPv4 except of the address shape \(hexadecimal\).
* IPv6 is also layer 3 addressing.
* IPv6 ranges also have a network and host address.

IPv4 is dotted decimal while IPv6 is hexadecimal.  
IPv6 subnet masks cannot be written the same way as IPv4 in decimals, hence usage of CIDR exclusively.

### Remarkable difference: The concept of a Global Address

Every IPv6 device will have multiple addresses but one global address \(public address\).

![Between a byte and a bit there&apos;s a nibble.](../.gitbook/assets/image%20%2827%29.png)

### Abbreviating and Expanding IPv6 Addresses

* You can only drop leading zeros, never trailing zeros.
* You can replace running groups of zeros with double colon **once** \(::\)

### Types of IPv6 addresses

| \# | Type | Binary | IPv6 |
| :--- | :--- | :--- | :--- |
| 1 | unspecified | 0000...000 | ::/128 |
| 2 | Loopback | 0000...001 | ::1/128 |
| 3 | Global | 001... \(first three\) | 2000::/3 \(2000 - 3fff\) |
| 4 | Multicast | 1111 1111... \(first eight\) | FF00::/8 |
| 5 | Link Local | 1111 1110 10... \(first ten\) | FE80::/10 |



