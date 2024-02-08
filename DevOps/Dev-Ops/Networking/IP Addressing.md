### DHCP:

DHCP (Dynamic Host Configuration Protocol) is a network management protocol used to dynamically assign an IP address to any device, or [node](https://www.techtarget.com/searchnetworking/definition/node), on a network so it can communicate using IP. DHCP automates and centrally manages these configurations rather than requiring network administrators to manually assign IP addresses to all network devices. DHCP can be implemented on small local networks, as well as large enterprise networks.
- It is based on client server model
- Works at Application Layer
- Dynamic IP allocation like for particular time give the IP
- DHCP IP address Range is known as scope(Range of IP like 172.10.0.0/24)
- BootP is another method to allocate the IP, but MAC address can be entered manually i BootP Tabl.
- DHCP is a dynamic BootP.
- It use UDP port at 67 and 68 Port at Transport Layer
- Destination Port/Listen    68
- Source Port /send req.     67
### DHCP can Provide..
- IP addresss 
- Subnet Mask
- Domain name
- Default Gateway 
- DNS Server Address
- Wins Server Address

### DORA:(Discover Offer Request Acknowledgement)
![[Pasted image 20240201183312.png]]


## Network Address Translation (NAT)

To access the Internet, one public IP address is needed, but we can use a private IP address in our private network. The idea of NAT is to allow multiple devices to access the Internet through a single public address. To achieve this, the translation of a private IP address to a public IP address is required. 
**Network Address Translation (NAT)** is a process in which one or more local IP address is translated into one or more Global IP address and vice versa in order to provide Internet access to the local hosts. Also, it does the translation of port numbers i.e. masks the port number of the host with another port number, in the packet that will be routed to the destination. It then makes the corresponding entries of IP address and port number in the NAT table. NAT generally operates on a router or firewall.