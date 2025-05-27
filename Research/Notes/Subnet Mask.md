A subnet mask is a 32 bit configuration value used by endpoints to interpret the network portion of their [[IPv4]] address

# How it is interpreted
The subnet mask is not represented as a decimal number, but as a series of 1s and 0s

11111111 11111111 11111111 00000000
Means the first 3 octets represent the network address
	The last octet represents the LAN address
# ![[Cidr]]

# How it is Configured
In the past, subnet masks were set by network admins manually.

However it is more common today for that to be automatically configured using [[DHCPv4]]

# Network Size
The remaining LAN bits, determine the max size of the [[LAN]]

8 bits means 256 devices can be  connected
9 bits means 512 devices can be connected
etc