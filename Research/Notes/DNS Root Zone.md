The root zone refers to the highest level DNS servers.
	There are 13 root zone servers operated by 12 independent organizations
	Organizations are labelled A-M
	These servers are actually virtualized to operate many many servers.
	One organization may operate 200 servers or 2 servers.
	Each instance of the root server is located on every continent

The DNS Root Zone is managed by #ICANN, and #IANA is responsible for the operations
	Just because you host a root server, does not mean you control it. Only IANA administrators can modify root servers

# Monitoring
Over 8 billion queries a day are made on a single root server

This makes big data extremely important

IANA requires all root servers to have probes to monitor metrics performance, and data
	This data is collected into every root server on the planet

# Root Server IPs
Root server IPs do change, but they are rare and when they do change a lot of work is done in the background.

# What do they even do
Root servers tell the DNS system where to find a given [[TLD]] name server.

For instance, .com may be evaluated to the Verisign TLD name server, since the Verisign TLD manages the .com TLD.