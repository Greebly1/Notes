Time To Live

An algorithmic technique used to prevent permanent cycling of a message through a network.

Most famously used with [[Notes/IP]] to prevent immortal messages from endlessly bouncing between routers.

# Hop Counter
TTL is often called a *hop counter*, but it doesn't count up.

When an IP packet is created it is given an 8 bit unsigned integer value as the max hops counter.

Each time the packet reaches a router or network device, the TTL hope counter is decremented.

If a router sees that an incoming packet's TTL is 0 (sometimes if it is close to 0), it ignores the packet and lets it die. 