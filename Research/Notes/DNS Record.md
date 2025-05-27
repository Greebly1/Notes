A DNS record is a small mapping between a domain name
ex
	example
and a IP

But this mapping is also given a record type, so that DNS resolvers can determine what the mapping means

For instance
if a DNS resolver is trying to find the mail server for the example domain, maybe the user is sending an email to example.com
	The DNS resolver will look for the IP pertaining to example's MX mail exchange server.
# Record Types
![[DNSRecords.png]]