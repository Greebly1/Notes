Due to private [[IPv4]] addresses, an endpoint within a LAN using IPv4 is not addressable outside the network.
	forget DNS servers, its actually just impossible to specify that specific computer.

This is only a problem if you need to host a server that listens on a port within a LAN.
	No connection requests will ever come in from outside the network since they cannot see you.

[[NAT]] servers offer a solution called port forwarding

Essentially a server inside a private IPv4 LAN can instruct the NAT server on the gateway to listen on port (n), and to forward all messages to the server inside the LAN.

This allows servers using private IPv4 LANs to make themselves visible to the outside world.