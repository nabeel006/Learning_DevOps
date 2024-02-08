Three way to preserve your IP.
1. Use the Private Addresses (10.0.0.0  - 172.16.0.0 - 192.0.0.0)
2. Use IPv6
3. Subnetting for if you want to use IPv4
Network within a network
Logically division of IP Addresses
 #### Why need ?
 Every Network having connected via router interface and every network should be having different Network Id.
 - Without subnetting, you might allocate a whole /24 network to each interface, leading to potential wastage.
- Subnetting enables more precise allocation, reducing the chances of leaving unused IP addresses.
- - Subnetting allows you to divide the original network into smaller subnets, like 192.168.1.0/25 and 192.168.1.128/25.
- Each subnet corresponds to a specific router interface or network segment.

**Example:** Let's say you have three departments - Sales, Marketing, and IT. Using subnetting, you allocate separate subnets for each department:

- Sales: 192.168.1.0/26
- Marketing: 192.168.1.64/26
- IT: 192.168.1.128/26

Each of these subnets can be assigned to a router interface connecting to the respective department. This targeted allocation minimizes IP address wastage and allows for efficient management and routing between departments.

Defult Addresses CIDR if there is any other CIDR means there is subnetting.
Class A     10.0.0.0/8
Class B     10.0.0.0/16
Class C     10.0.0.0/24



A subnet, or subnetwork, is a [network](https://www.cloudflare.com/learning/network-layer/what-is-the-network-layer/) inside a network. Subnets make networks more efficient. Through subnetting, network traffic can travel a shorter distance without passing through unnecessary [routers](https://www.cloudflare.com/learning/network-layer/what-is-routing/) to reach its destination.