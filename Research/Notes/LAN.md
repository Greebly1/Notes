Local Area Network

A LAN is a small network connected to the internet via a gateway  ![[Gateway]]
# Broadcast
LANs are broadcast networks, meaning that messages within a LAN are typically forwarded to all endpoints regardless of if it is the correct endpoint. 
	Broadcasts include the destination and source [[MAC Address]]
	It is like everyone is close enough to hear you speak, you don't need to send letters with their home address (IP address).

If an endpoint does not match the right MAC Address, it simply disregards the message.

# Subnet
The max size of a LAN is determined by [[Subnetting]]

ex:
	In an IPv4 LAN, a subnet mask of 24 means there can be up to 256 addressable endpoints (with some caveats)

The subnet mask tells endpoints when they need to go through the default gateway to speak to another computer.

# ![[Reserved Addresses]]