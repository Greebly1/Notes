IP Reservations
High priority network servers, such as web servers, game servers, etc may be given permanent *static* IP reservations. This prevents the IP from switching.
	Specify to the [[DHCP]] server which specific IPs are reserved.

# Especially in IPv6
Servers inside of a IPv6 LAN intended to be connected to from outside absolutely must have static IPs
	Imagine if the [[DNS]] server was still pointing to an old address lien.
	In action though, typically domain names are set to a proxy server.