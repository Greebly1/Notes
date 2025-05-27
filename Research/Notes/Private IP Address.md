AKA
	Link-Local IP Address

These are fake virtual IP addresses that are not based on any official IP leins from an ISP or RIR authority. They are locally managed.
# Port Forwarding
As such any local IP address is not addressable outside of the network. So servers cannot use private IP.

![[Port Forwarding]]

# Outbound Requests
Private IP addressed devices can still communicate with the greater internet by using [[NAT]]. A IP address translation and multiplexing server that runs on the gateway.

# Common Ranges
10.0.0.0/24
172.16.0.0/20
192.168.0.0/16 <-- most common