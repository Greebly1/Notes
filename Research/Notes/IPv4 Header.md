[[IPv4]] Internet protocol attaches a header to the message used at the [[Notes/IP]] layer of the #OSI stack.

![[IPv4Header.jpeg]]

The most important parts of the header are
- Source IP (Who is sending the message)
- Destination IP (Where to route the message)
- [[TTL]]
- Total length (helps to parse data payload)
- 16 bit header [[Checksum]]
	Used to ensure data is not corrupted or tampered with.

# Main Issues
IPv4 was invented at a time before the internet was as large as it is today
It has many issues
1. 32 bits is not enough addresses for mankind to continue developing networked machines, forcing us to develop [[NAT]]
2. Calculating and verifying the checksum slowed down networks a lot.

This lead to the creation of [[IPv6]], which solves all of its problems and is meant to eventually replace IPv4.
