## ifconfig Command
It is used to configure and display information about network interfaces on a system.
It is used at the boot time to set up the interfaces as necessary. After that, it is usually used when needed during debugging or when you need system tuning. Also, this command is used to assign the IP Address and netmask to an interface or to enable or disable a given interface.

 ****Syntax of `ifconfig`Command in Linux****

- **interface** is the network interface you want to configure or display information for (e.g., eth0, wlan0).
-  **options** are various command-line options that can be used to modify the behavior of ifconfig.
To view information about all network interfaces on your Linux system, simply execute the following command:

``` bash
ifconfig
```

``` bash
#display IP addresses associated with interfaces
ip addr show
#Adding a new address
ip addr add 192.168.0.1 dev eth0

The `dev` flag is used before designating which device or interface that the IP address is being set on.

#To remove an IP address from an interface
ip addr del 192.168.0.1 dev eth0
#Enable and disable an interface
ip link set eth0 up

#to disable:
ip link set eth0 down

#View the routing table
ip route show

#To add a static route, we use the following:
ip route add 10.5.5.10/22 via 192.168.0.1 dev eth0
#to delete static route:
ip route del 10.5.5.10/22
```
#### What is Public and Private IP in Linux

In the realm of networking, both in Linux and other operating systems, IP addresses are categorized as either public or private. These designations are crucial for facilitating communication between devices on a network, whether it’s the global internet or a local intranet. Let’s delve into the distinctions between public and private IP addresses in Linux.

## Netstat Command
The network statistics (`netstat`) command is a networking tool used for troubleshooting and configuration, that can also serve as a monitoring tool for connections over the network. Both incoming and outgoing connections, routing tables, port listening, and usage statistics are common uses for this command.


```bash
#To list all listening ports, using both TCP and UDP, use 
netstat -a

#List only UDP port connections
netstat -au

#List only TCP port connections
netstat -at
#List all actively listening ports
netstat -l
#finding the number of listening programs on a port.
netstat -ap | grep http
```

### Pull statistics by protocol
``` bash
netstat -s

#TCP stats
netstat -st
#UDP stats
netstat -su

#If all of this filtered data isn't for you, consider pulling the raw stats:
netstat --statistics --raw
```

### Display services by PID
``` bash
netstat -tp
```

### Show I/O by interface
```
 #view send/receive stats by interface
 netstat -i
```


# Tools for DNS name resolution problems
- ping
- nslookup
- dig
- host
## ping command
The `ping` command is a network utility tool used to test the reachability of a host (typically a computer or server) on an Internet Protocol (IP) network.

``` bash
ping www.example.com
ping 192.168.1.1

```
## ns-lookup Command:
It is used to query Domain Name System (DNS) servers to obtain domain name or IP address information.

``` bash
nslookup [options] [hostname or IP address] [DNS server]
```

## dig Command:
dig enables you to make manual name resolution queries. It provides an immense amount of detail about the results.
Generate forward lookups like this:

```shell
$ dig server01
```

Initiate a reverse lookup by using the `-x` option and the known IP address:

```shell
$ dig -x 192.168.1.101
```

Query the name server for specific record types by appending the type to the command:

```shell
$ dig example.com MX
	```


## host Command

Doing manual name resolutions with the `host` command are also straightforward.

Here is the basic syntax for a forward lookup:

```shell
$ host server01
```

Here's the syntax for a reverse lookup:

```shell
$ host 192.168.1.101
```

Querying for SOA records relies on the `-C` option:

```shell
$ host -C example.com
```

The `-t` option causes the `host` command to display the specified record type. The following example queries for the MX records of example.com:

```shell
$ host -t mx example.com
```

If you're not sure which record types you need or if you want to see them all, use the `-a` (any) option:

```shell
$ host -a example.com
```
