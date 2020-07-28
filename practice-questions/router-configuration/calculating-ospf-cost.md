# Calculating OSPF cost

![](../../.gitbook/assets/image%20%286%29.png)

**Scenario**

RouterA and RouterB is connected by FastEthernet Link  
RouterB and RouterC with Ethernet link.

\*\*\*\*

{% tabs %}
{% tab title="Question" %}
**What is the most likely cost value of the OSPF path from Router A to Router C**

A. 0  
B. 1  
C. 11
{% endtab %}

{% tab title="Explanation" %}
### \(C\) The cos**t is most likely 11.**

The cost of a link is based on the interface bandwidth and the reference bandwidth. It can be represented with the following formula:

$$
cost = reference bandwidth / interface bandwidth
$$

The higher the bandwidth, the lower the cost.  
The total cost is the sum of this function for every hop from source to destination  
  
  
In this scenario the calculation becomes the following:

`cost of hop 1 = 100 000 000 / 100 000 000 = 1  
cost of hop 2 = 100 000 000 / 10 000 000 = 10  
cost of hop 1 + cost of hop 2 = 1 + 10 = 11`
{% endtab %}
{% endtabs %}







