The first [[DHCP]] servers operated with [[IPv4]] addresses.

As part of configuration, a DHCPv4 server would tell every endpoint in a LAN what the [[Subnet Mask]] for their network was.

# Private IP
Most DHCPv4 servers actually managed private *virtual* IP addresses. 
That is, instead of loaning out official IANA IPv4 addresses, DHCPv4 servers loaned out fake virtual IPv4 addresses to later be translated at the gateway by a NAT server.