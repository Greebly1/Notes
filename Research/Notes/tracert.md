A #Command used to diagnose #network problems.

	tracert example.com

	tracert 120.420.69.4

Tells you the path that a [[ping]] takes through the internet
![[TracertExample.jpg]]

# Options
-4
Use IPv4 only
-6
Use IPv6 only

etc

# How it works
Tracert uses the [[ICMP]] time exceeded message, which occurs after a packet's [[TTL]] has expired (a packet has ran out of hops).

Tracert can map each hop on a path to a destination by changing the original packet's TTL. 
A starting TTL of 3 will show the third hop that the packet reaches.
tracert continues by incremening the TTL for each subsequent hop until it reaches the destination.

Some hops will not respond if they are not configured to reply to ICMP messages. tracert will note these as unknown.