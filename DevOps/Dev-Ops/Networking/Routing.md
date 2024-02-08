### Components of Routing:
##### 1. Path Determination
- Static Routing
- Dynamic routing 
- Default Routing
##### 2. Path Forwarding


## Routing Updates
- Periodic
- Topology Changes


AD (Administrative Distance) 
Lower value has higher Priority.
Always AD 0 of the same network with the router.


**Types of Routing:**

1. **Static Routing:**
    
    - **Description:** In static routing, network administrators manually configure the routing table on each router in the network. The routing paths remain constant unless the administrator makes manual changes.
    - **Advantages:** Simple to configure and requires less overhead.
    - **Disadvantages:** Not adaptive to network changes, and manual intervention is needed for updates.
2. **Dynamic Routing:**
    
    - **Description:** Dynamic routing protocols enable routers to automatically exchange information about the network's topology and make real-time decisions about the optimal path for data packets.
    - **Advantages:** Adapts to changes in the network, scalable, and reduces manual configuration.
    - **Disadvantages:** May involve more overhead and complexity.
3. **Default Routing:**
    
    - **Description:** Default routing is used when a router does not have specific information about the destination network. Instead, it forwards packets to a default gateway or next-hop address.
    - **Use case:** Often employed in smaller networks where a single router connects to the broader network.
4. **Dynamic Host Configuration Protocol (DHCP) Routing:**
    
    - **Description:** DHCP routing assigns IP addresses dynamically to devices in a network and can include information about the default gateway and DNS servers.
    - **Use case:** Commonly used in local area networks (LANs) to automate IP address configuration.
5. **RIP (Routing Information Protocol):**
    
    - **Description:** RIP is a distance vector routing protocol that uses the hop count as the metric to determine the best path. RIP is a simple and widely used protocol.
    - **Use case:** Suitable for small to medium-sized networks.
6. **OSPF (Open Shortest Path First):**
    
    - **Description:** OSPF is a link-state routing protocol that calculates the shortest path to a destination based on the network topology. It's more scalable and adaptable than RIP.
    - **Use case:** Commonly used in large, complex networks.

## Routing Metrics:
- Bandwidth 
- Delay
- Hope Count
- Cost
## Type of Dynamic Routing:
- Distance Vector Routing (Decides Path on the basis of hope count)
- Link State routing Protocol(Very intelligent,Build its own internal map topology,triggrered Updates send to neighbours)
- (OSPF)Dijkstra Shortest Path Algorithm by the other router who know the path is break from other routers.It uses the badthwidth and then find the cost and check the suitable cost to reach the destination.


![[Pasted image 20240202183508.png]]
## ENI: Elastic Network Interface 

Having its own Private and MAC addrss .Its cannot be deatach from the EC2 Intsance in any situation.
It is a component that helps your EC2 in the Network.
ENI are in primary and for the secondary it depends on your own need.


### Internet Control Message Protocol (ICMP):

The Internet Control Message Protocol (ICMP) is a network layer is used on network devices, such as routers . ICMP is crucial for error reporting and testing, but it can also be used in Distributed [[Denial-of-service (DoS) attacks]].
The primary purpose of ICMP is for error reporting. When two devices connect over the Internet, the ICMP generates errors to share with the sending device in the event that any of the data did not get to its intended destination. For example, if a packet of data is too large for a router, the router will drop the packet and send an ICMP message back to the original source for the data.

The commonly used terminal utilities traceroute and ping both operate using ICMP.

### Traceroute:
The traceroute utility is used to display the routing path between two Internet devices.
 a traceroute also reports the time required for each hop along the way. This can be useful for determining sources of network delay.
### Ping:
The ping utility is a simplified version of traceroute. A ping will test the speed of the connection between two devices and report exactly how long it takes a packet of data to reach its destination and come back to the sender’s device.
==**The journey between one router and another is known as a ‘hop’**==

All data sent over the Internet is broken down into smaller chunks called "packets."

##### Address Resolution Protocol (ARP):
 Our mission is to get the destination MAC Address which helps in communicating with other devices. This is where ARP comes into the picture, its functionality is to translate IP addresses to Physical Addresses.
 ![[Pasted image 20240202125351.png]]
