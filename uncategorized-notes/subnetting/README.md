# Subnetting

## The three-step subnetting process

### 1. Convert the number of networks to binary

Remember, subnetting is like slicing a pizza. We got to know how many slices we want to end up with.  
So the number of slices -&gt; number of networks should be converted to binary.  
  
Use this table

| Binary bits | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Decimal value by position | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |

**Thought process**  
You need 50 networks. 50 fall in-between 64 and 32 in the table.  
Count the bits from the highest number below 50 in the table \(32\).  
32.. 16.. 8... 4.. 2.. 1.. gives 6 bits!



###  2. Reserve bits in the mask and find your increment

The CIDR notation /XX indicates the count of bits in the subnet mask, where XX is the amount.  
This is how a /24 looks like:

| Binary bits | 1 1 1 1 1 1 1 1 | 1 1 1 1 1 1 1 1  | 1 1 1 1 1 1 1 1 | 0 0 0 0 0 0 0 0 |
| :--- | :--- | :--- | :--- | :--- |
| Decimal value | 255 | 255 | 255 | 0 |

If you count the ones you will see there are 24 ones.

### 3. Use increment to generate network ranges



## Cheat Sheet

![](../../.gitbook/assets/image%20%2818%29.png)

## Subnet characteristics

**Classful addressing**

When IP-addressing was developed there were 3 original classes

| Class | First octet range | Octets representing network port | Binary |
| :--- | :--- | :--- | :--- |
| Class C | 192 - 223 | first three octets | The value of first two binary places in the first octet must be 11. |
| Class B | 128 - 191 | first two octets | The value of first two binary places in the first octet must be 10. |
| Class A | 1 - 126 | first octet | The value of first binary places in the first octet must be 0. |

