The IPv4 address is a logical network address that identifies a host. It is  configured within a LAN for local communication. it is how  a host is able to communicate with other devices o the internet. The ipv4 address assigned to the network interface connection for a host. The connection is a NIC installed in the device .every packet has a source and destination 1PV4 address to ensure the information get to the correct address.
IPv4 addresses are 32 bits in length which is difficult to read. The 32 bits are grouped into four 8-bit bytes called octets like this:
11010001.10100101.11001000.00000001. The 32-bit IPv4 address is hierarchical and is made up of two parts, the network and the host.Both networks have the subnet mask 255.255.255.0. The subnet mask is used to identify the network on which the host is connected.
As an example, there is a host with an IPv4 address 192.168.5.11 with a subnet mask of 255.255.255.0. The first three octets, (192.168.5), identify the network portion of the address, and the last octet, (11) identifies the host. This is known as hierarchical addressing because the network portion indicates the network on which each unique host address is located. Routers only need to know how to reach each network, rather than needing to know the location of each individual host.
Muoltiple  logical networks can exist in one physical networkif the network portion of the logical netowrk host adressess is diffent.The hosts with the same network number in their IPv4 addresses will be able to communicate with each other, but will not be able to communicate with the other hosts without the use of routing. 


the ways of sending  a packet from a source  to destination
Unicast transmission refers to one device sending a message to one other device in one-to-one communications.A unicast packet has a destination IP address that is a unicast address which goes to a single recipient. A source IP address can only be a unicast address, because the packet can only originate from a single source. IPv4 unicast host addresses are in the address range of 1.1.1.1 to 223.255.255.255.
Broadcast transmission refers to a device sending a message to all the devices on a network in one-to-all communications.A broadcast packet must be processed by all devices in the same broadcast domain. A broadcast may be directed or limited. A directed broadcast is sent to all hosts on a specific network. A limited broadcast is sent to 255.255.255.255.
Multicast transmission reduces traffic by allowing a host to send a single packet to a selected set of hosts that subscribe to a multicast group.

Types of IPV4 Address
A public IP address is an address that is globally routable across the internet.
A private IP address is an address used inside a private network.
There are three reserved private IPv4 address ranges defined by RFC 1918.;
Range 1
10.0.0.0/8
10.0.0.0 – 10.255.255.255
Often used in large organizational networks.

Range 2
172.16.0.0/12
172.16.0.0 – 172.31.255.255
Another private address block used in internal networks.

Range 3
192.168.0.0/16
192.168.0.0 – 192.168.255.255
Very common in home and small office networks.

the /8, /12 and /16 are called CIDR prefix lengths.CIDR stands for Classless Inter-Domain Routing.The number tells us how many bits of the IPv4 address are used to identify the network portion.

private IPv4 addresses became important because the world was running out of available IPv4 addresses.IPv4 provides approximately 4.3 billion possible addresses.

As more computers and devices connected to the internet, the available address space became insufficient.

Private addresses helped solve this problem because different organizations could reuse the same private addresses internally.IPv4 provides approximately 4.3 billion possible addresses.

As more computers and devices connected to the internet, the available address space became insufficient.

Private addresses helped solve this problem because different organizations could reuse the same private addresses internally.

Special Use IPv4 Addresses.
Loopback addresses:These are special addresses used by a host to direct traffic to itself. For example, the ping
Link-local addresses:A link-local address is a special IPv4 address that a device can automatically assign to itself when it cannot obtain an IP address through its normal configuration methods.
This is also known as an APIPA address.APIPA means Automatic Private IP Addressing.

Before modern IP addressing methods were introduced, IPv4 addresses were divided into different classes.This system was called Classful Addressing.networks had different sizes, so they needed different amounts of IP addresses.
Class A                                                       
1.0.0.0 – 126.255.255.255
Designed for very large networks.
- Default subnet mask: 255.0.0.0
- CIDR prefix: /8
- Hosts per network: 16,777,214

- Class B
128.0.0.0 – 191.255.255.255
Designed for medium-sized networks.
- Default subnet mask: 255.255.0.0
- CIDR prefix: /16
- Hosts per network: 65,534

- Class C
192.0.0.0 – 223.255.255.255
Designed for small networks.
- Default subnet mask: 255.255.255.0
- CIDR prefix: /24
- Hosts per network: 254

- Class D
224.0.0.0 – 239.255.255.255
Used for multicast communication, not ordinary host addressing.

Class E
240.0.0.0 – 255.255.255.255
Reserved for experimental or future use


These notes document my learning from Cisco Networking Academy as I continue developing my networking knowledge.


