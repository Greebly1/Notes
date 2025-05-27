Network Address Translation

A server protocol that runs on a gateway responsible for translating private [[IPv4]] addresses from a LAN into a public [[IPv4]] address, essentially using itself as a proxy.

# How it works
Devices in a LAN will be given fake virtual IP addresses. 
	[[Private IP Address]]
The NAT server is located on a gateway that has been given a regular IPv4 address by an ISP
	Public IP Address
	
All LAN devices communicate with each other in their network using the fake virtual addresses just fine.

When they send a message to the gateway, the NAT server replaces the *source address* in the [[IPv4 Header]] with the gateway's public IP address.
	It then replaces the [[TCP Port]] or [[UDP]] source port with some random ephemeral port available to the gateway.

The NAT forwards the packet like a proxy server.
When/if it receives a response on that port, the NAT server, does the opposite, it replaces its IP address with the private IP Address, and replaces the TCP/UDP port with the correct one before handing it back to the routing algorithm to send to the correct endpoint on the LAN.

# Proxy Similarities
NAT servers are *similar* to [[Proxy Server]]s, but they are not quite the same.

Similarities
- Both mask the IP address on the internet
Differences
- NAT does not cache data

# ![[Port Forwarding]]