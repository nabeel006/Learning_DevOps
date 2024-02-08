## Firewall:
A firewall is a network security device or software that monitors, filters, and controls incoming and outgoing network traffic based on predetermined security rules. Firewalls act as a barrier between a trusted internal network and untrusted external networks, such as the internet. They are essential for protecting networked systems from unauthorized access, cyber attacks, and other security threats.

Types of Firewalls:

1. **Packet Filtering Firewalls:**
    
    - Examines packets of data and filters them based on predefined rules.
    - Rules are typically based on source and destination IP addresses, port numbers, and protocol types.
    - Simple and efficient but may not provide advanced inspection capabilities.
2. **Stateful Inspection Firewalls:**
    
    - Keeps track of the state of active connections and makes decisions based on the context of the traffic.
    - Monitors the state of active connections and allows or denies traffic based on the state table.
    - Offers better security than packet filtering by considering the state of the connection.
3. **Proxy Firewalls (Application Layer Gateways - ALGs):**
    
    - Acts as an intermediary between internal and external systems.
    - Its checks the Data within the packet and check the valid uses details and then create session for the user if information is correct.
    - It scan deeply and works on application layer.
    - Can provide content filtering and additional security features but may introduce latency.
4. **Next-Generation Firewalls (NGFW):**
    
    - Integrates traditional firewall features with additional functionalities such as intrusion prevention, application-layer filtering, and deep packet inspection.
    - Offers more advanced threat detection and prevention capabilities.
5. **Unified Threat Management (UTM):**
    
    - Combines multiple security features into a single device or software solution.
    - Typically includes firewall capabilities, antivirus, intrusion detection/prevention, VPN, and content filtering.


### Linux Firewall:

 A Virtual wall in the security system world is designed to protect our system from unwanted traffic and unauthorized access to our system. The security system in Linux OS is known as Linux Firewall, which monitors and governs the network traffic (outbound/inbound connections). It can be used to block access to differentIP addresses, Specific sunsets,ports virtual points where network connections begin and end), and services. We have a daemon’s name called Firewalld which is used to maintain the firewall policies. A dynamically managed firewall tool in a Linux system is known as Firewalld, it can be updated in real-time if there are any changes in the network environment.

### Some rules of Firewall
#### **Rule 1: Allowing SSH (Secure Shell or Secure Socket Shell) traffic**
By using this we can allow all incoming traffic on the SSH port so that we can connect to the system remotely.
``` bash
   sudo firewall-cmd --zone=public --add-services=ssh --permanent
   sudo firewall-cmd --reload
```

#### **Rule 2: Allowing incoming traffic on a specific port**
We are allowing traffic on a specific TCP port 8080 you can replace it with requirements.

```bash
sudo firewall-cmd --zone=public --add-port=8080/tcp --permanent
sudo firewall-cmd --reload
```

#### **Rule 3: Blocking incoming traffic on a specific IP address**
We are blocking incoming traffic on IP 192.168.52.1 you can replace it with your requirements.
```bash
sudo firewall-cmd --zone=public --add-rich='rule family="ipv4" source address="192.168.52.1" reject'
sudo firewall-cmd --reload
```



### Types of Linux Firewalls

### Iptables:

Linux-based software that performs manipulation functions, packet filtering, and NAT (network address translation) is known as Iptables. With the help of Iptables which allows system administrators to control incoming and outgoing traffic by setting up the rules. 

When a packet is received in a Linux base system, it has to go through the chains and tables in the iptables firewall. The most commonly used tables are filter and nat but we have five predefined tables in iptables (raw, nat, filter, security, and mangle).