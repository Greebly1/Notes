[[IPv6]]
StateLess Address Auto Configuration
	Alternative to [[DHCP]] for IPv6 networks

# 1 Router Advertisements
Abbreviated (RA)
Special network control signals used to inform devices in a network what their network prefix is, their default gateway, and other control information. Does not include DNS configuration
	Since we have no other way of knowing their network prefix
**Control flags**
- M flag (Managed flag) → Use DHCPv6 for addressing.
- O flag (Other Config flag) → Use DHCPv6 for extra settings (like DNS).
**Address Lifetimes**
	A RA also informs devices of how long their SLAAC IPv6 IPs are valid for before needing to repeat the authentication procedure.

Devices may also probe routers to determine their network prefix if they do not know it by sending a **Router Solicitation**

# 2 Address Generation
Devices use the network prefix to generate a device address to fit into the network.
- **EUI-64** (based on MAC address, discouraged for privacy reasons)
- **Randomly generated** addresses for privacy (preferred)

# 3 Duplicate Address Detection
abbreviated (DAD)
A broadcasted protocol designed to discover if their address is unique within the LAN. 
	If a device responds, saying it is a duplicate address the device returns to step 2 to generate a new address to try again.

# 4 Final Configuration
Device broadcasts what address it is using, and the default gateway adds it to the routing table.

# Cons
- Does not include DNS configuration
- Distributed instead of centralized control from DHCPv6
