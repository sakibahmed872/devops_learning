# Class One
## What is DevOps ?
DevOps is borned to handle scaling and monitoring traffic. DevOps is not for either Development portion or Operations. DevOps is mostly connect to developments and operations. Developments knowledge  is more important here. DevOps should know most of the technical knowledges of development phase.

# What I will learn

* Docker
* Kubernates
* Microservices Design
* Scaliblity

## DNS Query
to make a DNS query, copy the following command to the terminal and hit enter.

```bash
 dig facebook.com
 ```

#### Output
![DNS Query](https://github.com/sakibahmed872/devops_learning/blob/master/Class%20One/dns_query.png)

## What is ARP?
ARP is a Address Resolution Protocal. What does it mean actually ? 

ARP is the most important Communication protocol of Network Layer. It translates Logical address to Physical address, known as MAC Address. 

ARP has been used in IPV4 technology where IP address is 32 bit but MAC address is 48 bit. But in the IPV6 technology where IP address is 128bit, ARP has been repleaced by Neighbor Discovery protocol.


Important topic related to ARP:
* ARP Cache
* ARP Cache timeout
* ARP request
* ARP response/reply

\* Reverse ARP is being used when host computer/machine don't know their own IP address. 

___


## Routing Table
A routing table is a set of rules that is used to determine where the packet is traveling. 

Example of Routing Table:

|Network destination | Netmask| Gateway | Interface |
|---|---|---|---
|0.0.0.0|0.0.0.0|192.168.0.1|192.168.0.100|
|127.0.0.0|	255.0.0.0|127.0.0.1|127.0.0.1|
|192.168.0.0| 255.255.255.0|	192.168.0.100| 192.168.0.100|
|192.168.0.100|	255.255.255.255|	127.0.0.1|	127.0.0.1|
|192.168.0.1|	255.255.255.255|	192.168.0.100|	192.168.0.100|



## Classless Inter-Domain Routing- CIDR
CIDR is IP addressing scheme that improved the allocation of IP address. Previously we used Classes to define a IP range. But CIDR removes it and come with a solution to define the IP address in a way where we can find or calculate many important things like number of hosts, sebnet mask from CIDR. For example, 192.168.0.0/16 IP address has a 16 bit blocks. It means 16 blocks will be the network part and rest of the will be host part. CIDR is also used in IPV6 standard but highest number of blocks increase from 32 to 128. 


#
## Namespaces
>Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources and another set of processes sees a different set of resources. The feature works by having the same namespace for a group of resources and processes, but those namespaces refer to distinct resources. - [Wikipedia]("https://en.wikipedia.org/wiki/Linux_namespaces")

Namespaces is one of the most exciting feature of Linux Kernel that seperates Linux from others. There are 8 types of namespaces in the linux kernel. 


### Network Namespace
Network Namespace creates a separate Network world inside the main computer but separate from Host Namespace. A network namespace is a black box for host namespace. It means Host Namespace don't have any access to that network namespace and vise-versa. Host namespace and any network namespace can be connected through virtual ether to transfer data or packet. In a linux system, multiple numbers of network namespaces can be created where necessary. 











___
___
### Reference

* [Address Resolution Protocol](https://en.wikipedia.org/wiki/Address_Resolution_Protocol)
* [Address Resolution Protocol (ARP)](https://searchnetworking.techtarget.com/definition/Address-Resolution-Protocol-ARP)
* [Linux Namespaces]("https://en.wikipedia.org/wiki/Linux_namespaces")