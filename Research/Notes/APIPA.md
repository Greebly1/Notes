Automatic Private Internet Protocol Addressing

A fallback system that allows computers to assign themselves an [[IPv4 Address]] if they are unable to acquire one from a [[DHCPv4]] server.

# Address Range
A device will just randomly choose an address in the range
169.254.0.1 - 169.254.255.25

Uses a [[Subnet Mask]] of 16

It then uses [[ARP]] to relay that IP to the rest of the APIPA network.

# APIPA Network
Since APIPA has a different subnet mask, (and network address) from the actual LAN, APIPA devices cannot communicate with actual IP loaned devices on the network unless they are directly connected.
	This is because all APIPA traffic is broadcast, and if a device wants to speak to an APIPA device it sends it to the default gateway (since it has a different subnet and network address), and routers block all broadcasts.