**Hardware:

We can touch feet it

But Cannot be change  

FirmWare:

It is created on the time when hardware is created .It helps to communicate the diff hardware to each other .It also cannot be changed ,can be updated but cannot be deleted.

Like App store APP version, android version, OS update, Firmware or hardware update.

Like hardware, understand the Bootable flash on a new laptop.

It is too small for supporting the system and how the OS works.

Every Hardware has its Firmware and like the BIOS of Computer and cannot be accessible.

It is also a system Software.

  

Software:

![](https://lh7-us.googleusercontent.com/uyHbloK4MYaXPWsoMILuf4NqheNvOHZsWZb8ZeFE3kvW0UaQ5rYkZGustcxGd51H1LPkinLsxEJHXobOywnpLznxBZPTC9IX9k-tQQM79ParTbPSSdKrbJWN79BQUaXgi3U4OArRccjjaxEUi-4mWiY)

  
  
  

Simplex (TV only receive signal)

Half Duplex(Walkie Talkie, army cell phone like Ok and over)

Full Duplex (Telephone call)

  
  

# OSI Model:

The OSI (Open Systems Interconnection) model is a framework with seven layers that standardized how different computer systems communicate. From the physical connection (Layer 1) to end-user services (Layer 7), each layer has a specific role in managing aspects like hardware, addressing, routing, and application-level interactions. It simplifies understanding and troubleshooting network processes.

  

It is a reference model.

(APSTNDP)

First Layer depends on which side you like on sender then the first layer is Application Layer and for receiver side the first layer is Physical Layer.

  

![](https://lh7-us.googleusercontent.com/gPqbqumG-Nwsr6LnBEcrA9zvQujxIAn-zGnuH9h9lk5f6TvKHbvIWRGuO-yFkdlrKeqLIWNzEmBj7_W2CgF7E6QrqvJ0IkNhDbyaOKYnRFp6E2PNNB_mkCXFfywMkPV2Owgxh7Grhltleqq1dr4VaSk)

First three layers are Software Layer and Last three layers are Hardware Layer and Transport Layer is the heart of these 6 Layers It supports connectivity between these.

  

ApplicationLayer:

FTP,HTTP,Telnet Protocol Works here.

  

Presentation Layer:

Encryption and Decryption

Like (song.mp3 , file.docx  and when we click on any of the file the Extension tells that file will be present in MS Office or Music Player)

How we present the data

  

Session Layer:

End to End Connection. It is responsible from the sender Session layer to Receiver Session layer. If there is any issue occurring it gets the notification that data is received .

Like Mail sent successfully.

Transport Layer:

  

Segmentation

Provide the Logical Ports for data .

TCP/UDP  Protocols

Network Layer:

IP Addressing sender and receiver IP

Routers are on these layers.

  

Data Link Layer:

Error Detection and Correction Capability and flow control.

Physical Layer:

All Data Converts into bits and transmits to the receiver ith the help of wireless or wire network.

  
  
  
  

![](https://lh7-us.googleusercontent.com/9vQ5pm3PBs0qI1Hkx5PkVXDKPTQzgXlKulKGICO-9XSzOJr3mr1vU47aLqpL4KESFMCJGQ_v08MSYYUSFzhRx989TEwZ0imvykiPzsiPiZuHK0oLN6SRB_IApgWZDsfskuqUmv6oLA_H12lOJAhqVvs)

  
  
  

TCP/IP Model:

  

When two devices communicates over the internet TCP/IP is using there.

TCP: Transmission Control Protocol

IP: Internet Protocol

  
  

TCP (acknowledge os your connection)

IP(Source and Destination Path, which route)

  
  

Our concerns are to omit the Hardware dependent Communication that's why we use Model.

  

There is no relation between OSI and TCP/IP .

For understanding the Networking OSI is the best approach.

  

Two Key Points in TCP

End Node Verification:

The two end point of data transfer are responsible for making sure it was successful

No centralized control system

  

DYnamic Routing

  

End Nodes can transfer data over multiple paths and over the n/w choose the best path for the data transfer .

  
  
  

Network Facing Some Issues:

  

Addressing (IP and Mac Address)

Routing(Should to know about path)

Name Resolution  (DNS)

Follow and error Control (Fast sending but low receiving Packets leads to packet loss)

Interoperability

  
  
  
  

All these Are solve by TCP/IP

  
  

![](https://lh7-us.googleusercontent.com/zPISNWXF72VY1oughoH6i_XoHa85CS2bXnwHaSiihzIWZ6eExrLa6PlTmw5teaP-fMjJIrSDJCMCVZ1D-SXz5stSVNx7_g0krRQ_BOLEdYI89mPIY06Ryz829MiqiYEGG0Ru_IPiLqmKimvcTxL4JTM)

- Physical Layer:
    

- Ethernet
    
- USB
    
- HDMI
    

- Data Link Layer:
    

- PPP (Point-to-Point Protocol)
    
- HDLC (High-Level Data Link Control)
    
- MAC (Media Access Control)
    

- Network Layer:
    

- IP (Internet Protocol)
    
- ICMP (Internet Control Message Protocol)
    
- OSPF (Open Shortest Path First)
    

- Transport Layer:
    

- TCP (Transmission Control Protocol)
    
- UDP (User Datagram Protocol)
    

- Session Layer:
    

- NetBIOS (Network Basic Input/Output System)
    
- PPTP (Point-to-Point Tunneling Protocol)
    
- RPC (Remote Procedure Call)
    

- Presentation Layer:
    

- SSL/TLS (Secure Sockets Layer/Transport Layer Security)
    
- JPEG (Joint Photographic Experts Group)
    
- GIF (Graphics Interchange Format)
    

- Application Layer:
    

- HTTP (Hypertext Transfer Protocol)
    
- FTP (File Transfer Protocol)
    
- DNS (Domain Name System)
    

  
  

- Application Layer:
    
- These protocols help to go over the internet.
    
- Like app skype interface  for the user
    

DNS

DHCP

HTTP

FTP

TFTP

SMTP

SNMP

- Transport Layer:
    

- TCP (Transmission Control Protocol)
    

- Connection Oriented
    
- Retransmission is also like if any package is missing then it will send again.
    
- It Performs the sequencing and segmentation of data. It also has an acknowledgement feature and controls the flow of Data through flow control system.End to end Establishment and then acknowledgment.
    
- Mostly used for non-real time data. Like send a mail may be read after 2 days etc all document data sent by TCP.
    
- Slower than UDP(extra work because of acknowledgment)
    
- It is more reliable(packet is successfully receive or not)
    

-   
    
- UDP (User Datagram Protocol)
    
- Connectionless protocol
    
- Used for real time applications like youtube streaming videos audio video calling. Hand to hand data transfer instantly.
    
- No retransmission is there (like if voice cut during the call then no voice will be deliver after again ) Any packet loss then no retransmission
    
- Faster than TCP
    
-   
    

- Internet Layer:
    

- Internet Layer parallels the function of OSI.
    
- Network it defines the protocol which is responsible for logical transmission of data over the entire network.
    
- IP(sender and Receiver Address)It is a connection oriented protocol.
    
- Routing
    
- IP (Internet Protocol)
    
- ICMP (Internet Control Message Protocol)
    
- OSPF (Open Shortest Path First)
    
- ARP(Address Resolution Protocol)
    
- RARP(Reverse Address Resolution Protocol)
    
- IGMP
    
-   
    

- Network Access Layer:
    

- Combination of Physical and Data Link Layer of OSI Model. It looks out for hardware address
    
- Ethernet
    
- USB
    
- HDMI
    

- Data Link Layer:
    

- PPP (Point-to-Point Protocol)
    
- HDLC (High-Level Data Link Control)
    
- MAC (Media Access Control)
    

  
  
  
  
  
  
  
  
  
  
  
  

# Layer Devices:

![](https://lh7-us.googleusercontent.com/QDTyZ62ujt5N3v2-OXmP29PkI3V4Wtwa2yovxAq3arMRnIHPzxz2IbZ3qx03qZePdCCGU3Kt5SlJ7QHfxcCP1f5hRjqyTjtO0FM1Xj2-s8NfL_LJ-IqzUUDAR1mOTFqinUnXYeH39PxlbAWYwqNwN_o)

  
  

Layer Devices:

  

Layer 1: Hub/Repeater

Layer 2: Bridge and Switch

Layer 3: Router and Layer-3 Switch

  

Layer(4,5,6,7): Reset Layer are working with Gateways and Gateways mostly work with    Application Layer

  
  

Hub: Operates at the physical layer, simply forwarding signals to all connected devices. It doesn't make decisions based on the content of the data. Example: Basic Ethernet Hub.

- Topology
    
- Data Transmission
    
- Broadcasting
    
- Collision Domain
    
- Simple and Unintelligent
    
- Security Concerns
    
- Half Duplex
    
- Single Collison Domain(on one way i used to send and recieve data)
    
- Cannot store Mac Address
    
- No table handling like switch and router
    
- LAN Device
    

  

Repeater:

It regenerates your signal and extends the signal strength .Like if the signal goes to 180 m then it helps for more like 180m strength .

No Mac Address store there.

  
  

Layer 2 Model:

Bridge:

  
  
  

Switch:

  

Full duplex

Maintain CAM Table

First Broad Cast and then Uni and Multi Cast

Every Port of switch is separate Collision Domain

Switch has one broadcast Domain

8/16/24/32/48 Ports

Slow Wire (100MBPs) Wireless(10Mbps)

  

Types of Switch

Store and forward:

Buffer and verify each frame before forwarding it .Little bit slow and very reliable

Cut Through Switch:

It sends the packet and just reads only the frame hardware address before starting to forward. No error Checking

Fragment Free:

Method to attempt to retain both Store and forward switch and cut through switch check only header 64 bytes.

Adaptive Switch:

It work as you want on the other three type.

  

POE Switch:

  
  

HUB, Bridge and  Switch are Networking Devices and they require the same network ID.Also they work in LAN like in an office. But for different network Communication we use Routers.

# Router:

  

Layer 3 Device 

WAN Device

Connect two or more networks

Internetworking Device.(Diff network ID communication through routere)

In Router every port has its own BroadCast Domain

Uses IP address Send in Form of Packets.

Maintain Routing Table

2/4//8Ports

Fast

  

Routers always connect with switches and PCs always connect with switches.

  

There are always two different network IDs for using the router.

Router is always used for communication between two different networks or over the internet.

  
  
  

# Gateway:

Gateway is a device used to connect the remote network with the host network. Generally it act as a entry or exit point.It generally operate at application layer.

  
  

Network Topology: (Design of network)

  

Network topology refers to the physical or logical layout of devices, nodes, and connections in a computer network. It defines how different elements of a network are arranged and how they communicate with each other.

- Bus Topology
    
- Star Topology
    
- Ring Topology
    
- Mesh Topology
    
- Tree Topology
    
- Hybrid Topology
    
- Fully Connected (Mesh) Topology
    
- Point-to-Point Topology
    

  
  

Network Types:

  

LAN : 

Highest MAx speed and Most Secure and router involves

Switch

Ethernet cable

Coaxial Cable 

Twisted Pair Cable

  

MAN (Will Be moderate)

Ethernet Cable

WAN (Min Speed and more vulnerable)

  

Using Routers

FiberOptic Cable

Satellite

  
  

Two Type of Network Address:

Physical Address:

MAC Address: 

Media Access Control. —-> Mobile

Physical Address         —-> Laptop or PC

Hardware Address       —-> 

BIA (Burnt in Address) —->CISCO Router Switch)

  
  

- Name of device
    
- Representation of Entity
    
- MAC Address is globally unique
    
- Laptop doesn't have a MAC Address but it is on the NIC (Network Interface Card).
    
- It can be changed if we change NIC of Laptop otherwise we cannot change the MAC address
    
- (A laptop can be connected to a network using NIC like Ethernet Cable, WIFI and Bluetooth.)So it has three MAC addresses.
    
- It is 48 bits long
    

It Divides into two parts:

OUI and Vendor Specific Address. And OUI is totally different so it differs with other MAC

- It is Represented in HexaDecimal Format and consists of 12 HexaDecimal Characters.
    

  
  

Logical Address:

  

We can reach it in the exact place with the help of this.

IP Address

Two types : IPv4 and IPv6

Further IPv4 having Public and Private Addresses

  

(32 Bit Logical Address) having 4 Octet and values from 0-255

  

IP Address consist on two parts….:

1. Network Id                   2. Host ID
    

![](https://lh7-us.googleusercontent.com/P2vNkOolM884lK8gj9A2Urpnliwl-Lxbs75OsH09HZOOVN30SCZ7FZsRrJQrVgwlvsqWEtYnQr5mlAuB_ju952pVDAemQ8FtebH9f_suXqP-3KIKptIoMim-GTz_wIvo3XUjNK_Xf5lCSDSkzfzpSV8)

  
  
  

127.0.0.0  is LoopBack address.Helps to check the computer NIC using command and Ping command. It is also known as LocalHost

  

![](https://lh7-us.googleusercontent.com/6v6VBFKUhL4OEzBxn_YS6EReqm-Opw3HTyLq5XHC6B2iubjJNonNPg7TTbPSIQCplBFVAT26bweDthw81CsLyew-bmpTgehxrM810QDmlJUjUa_ey1954985FD-YoLRkmn8o9j0VMCiukbIZ76W8nPc)

  

Network Class 

Network ID

Network Host

How to get SubnetMask from IP Addresss?

115.10.10.20

  

255.0.0.0 (Subnet mask)

![](https://lh7-us.googleusercontent.com/iI7ND0GZOFIAMjnnRSQ0JgoYfuVKGmAROWOoK7JANnWKfUblhnawhTs1EAFwD8VDw2yEsWo-rtnVDMgfkzhWRMw4Zp0tQweCZ4rRx-8JhEEgJck3nPUzLxEtZ0R9y9sReebYqQO6WZINsZ-JxmFfuEg)

  
  

Private Addressing:

Private addressing refers to the use of IP addresses within a private network that are not routable on the public internet. These addresses are reserved for internal use within an organization and are defined in RFC 1918. Common private address ranges include:

- 10.0.0.0 to 10.255.255.255
    
- 172.16.0.0 to 172.31.255.255
    
- 192.168.0.0 to 192.168.255.255
    

Public Addressing:

Public addressing involves the use of globally unique IP addresses that are routable on the public internet. These addresses are assigned by Internet Assigned Numbers Authority (IANA) to Internet Service Providers (ISPs) and other organizations. Public addresses are necessary for devices to communicate directly over the internet.

When a device in a private network needs to communicate with a device on the internet, the private address is translated into a public address by a router using NAT. This enables communication over the internet using a single public IP address, helping conserve the limited pool of available public IP addresses.

  
  
  

We have to buy the Public IP and Private IP free of cost.

  
  

How to calculate the public address?

  

176.10.0.0 (Network Address) Host Part is 16 Bits

  

BroadCast ID : Reserved for specific tasks for example if you want to send a message to the whole network who are connected to this network to inform about vocation etc.

  
  

150.10.20.0

150.10.0.0  (Network ID)

  

150.10.255.255(Broad Cast)

  

See total bits for host: 

No of Hosts=  2^16 - 2

  
  
  

# IPv4 Header:

The IPv4 (Internet Protocol version 4) header is a fundamental component of the IPv4 protocol suite and is used to facilitate communication between devices on a network. It is a fixed-size, 20-byte header that provides essential information for the transmission of data packets. Below is an explanation of the various fields in an IPv4 header along with an example:

IPv4 Header Fields:

1. Version (4 bits): Indicates the version of the IP protocol being used. For IPv4, this field is set to 4.
    
2. Header Length (4 bits): Specifies the length of the header in 32-bit words. The minimum value is 5 (indicating a 20-byte header), and the maximum is 15.
    
3. Type of Service (8 bits): Originally designed for specifying the quality of service, it is rarely used today. Differentiated services (DiffServ) has largely replaced this field.
    
4. Total Length (16 bits): Indicates the total size of the IP packet, including the header and data. The maximum value is 65,535 bytes.
    
5. Identification (16 bits): A unique value assigned to each fragment of a packet when it is fragmented during transmission.
    
6. Flags (3 bits): Flags used for fragmentation control. These include the "Don't Fragment" (DF) flag, the "More Fragments" (MF) flag, and a reserved bit.
    
7. Fragment Offset (13 bits): Indicates the position of the fragment in the original packet, measured in 8-byte units.
    
8. Time to Live (TTL) (8 bits): Represents the maximum number of hops a packet can traverse before being discarded. It prevents packets from circulating endlessly in the network.
    
9. Protocol (8 bits): Specifies the protocol used in the data portion of the packet (e.g., TCP, UDP, ICMP).
    
10. Header Checksum (16 bits): A checksum for error-checking the header.
    
11. Source IP Address (32 bits): The IP address of the sender.
    
12. Destination IP Address (32 bits): The IP address of the intended recipient.
    
13. Options (variable): An optional field for various control options. It is rarely used and adds variable length to the header.
    

  
  

![](https://lh7-us.googleusercontent.com/d6owBDFHqZYBT4fLgHDLwGNENXnovedC6e2wTaTsBPC28YB2QhbSLYG9eWl6MuX59VeYKGxJ_c-uRvo2j7lA2eXeO0jX_Gfxn19KhXJKIYWIGDJRHR6SbiFbGkqltk8XL0qavCeqLEcZvGVFTQZivi0)

  
  

# Subnetting:

  
  

The Internet Control Message Protocol (ICMP) is a [network layer](https://www.cloudflare.com/learning/network-layer/what-is-the-network-layer/) protocol used by network devices to diagnose network communication issues. ICMP is mainly used to determine whether or not data is reaching its intended destination in a timely manner. Commonly, the ICMP [protocol](https://www.cloudflare.com/learning/network-layer/what-is-a-protocol/) is used on network devices, such as [routers](https://www.cloudflare.com/learning/network-layer/what-is-a-router/). ICMP is crucial for error reporting and testing, but it can also be used in Distributed [denial-of-service (DDoS) attacks](https://www.cloudflare.com/learning/ddos/what-is-a-ddos-attack/).**