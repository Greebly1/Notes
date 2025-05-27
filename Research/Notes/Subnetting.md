A sub-network is a network inside a network.

Subnetting is used **extensively** by the internet
	It gives the internet more structure

# Mask
Subnetting is achieved and configured by using [[Subnet Mask]]s
	In IPv6 it uses [[Network Prefix]]es

These masks split an [[IP Address]] into two parts
	Network address
	Host address
ex:
	IPv4 address 16:2:10:5/24
	Subnet mask of 24

# Network Address
Using the mask 24

   16          :        2        :      10        :       5
00010000 : 00000010 : 00001010 : 0000101
/24
11111111 : 11111111 : 11111111 : 0000000

The mask tells us that 
16:2:10 is the network portion, meaning the entire network is locatable using just that address

# Host Address
   16          :        2        :      10        :       5
00010000 : 00000010 : 00001010 : 0000101
/24
11111111 : 11111111 : 11111111 : 0000000

The mask tells us 
5 is the host address, meaning within a given network, endpoint 5 is what this address points to

# Mask Memorization
In practice, devices do not need to send their subnet mask for each message. Routing tables and clever algorithms remember what the subnet mask for each network is.
	Routers keep track of what the subnet mask is for each port they speak to, they route traffic based on the closes matching address.

# Gateway Forwarding
Before an endpoint sends a message, it checks the destination IP
If the network portion of the destination IP does not match the current network portion of their IP, it will forward the message to the default [[Gateway]].