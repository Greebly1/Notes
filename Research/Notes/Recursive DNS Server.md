Most DNS servers configured to be the default DNS server of an endpoint is a recursive DNS server.

That is, it odes not perform DNS infrastructure services such as being an [[Authoritative Name Server]], but it performs a recursive DNS query.

# Recursive Query
The DNS recursive query sums up the entire DNS infrastructure
Lets use the example
	example.com

1. First ask the [[DNS Root Zone]] for the IP of a .com [[TLD]] server
2. Ask the TLD server for the [[Authoritative Name Server]] of the domain, example
3. Ask the [[Authoritative Name Server]] for the IP address for that server or any subdomains

It's possible for even further recursion, if an authoritative name server does not know the IP, it may point to another authoritative name server.
This recursive query continues until it either
	Finds the IP for example.com
	or
	Decides it has failed and returns an error