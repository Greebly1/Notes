Domain Name Service

# Problem
To access resources and servers on the internet, computers need to know the [[IP Address]] of the service they are accessing.
	They need to know the address of the service

**This is not something humans can memorize easily**

# Solution
Humans want to memorize names
	We call these names, [[Domain Name]]

We simply need some kind of service that can translate a name into an IP address.
	Locate the IP address of the (name) service

Thus DNS is born

# DNS
DNS works like a *phone book*, every computer is configured to have a DNS server that is asks when translating domain names.

The DNS protocol begins when a user inputs a domain name into a search engine
	EX: http.wikipedia.org into Google Chromium

The search engine will use network configuration information to ask the default DNS server to find the IP address of the domain name *wikipedia.org*

The DNS server that receives this will check its database
	If it has the IP for the domain it will send it back
	If not, that DNS server will ask another DNS server for the IP for *wikipedia.org*, eventually returning it all the way back to the first computer

The computer now knows the IP address of *wikipedia.org*, and can now try talking to Wikipedia directly.

# DNS Configuration
Every computer needs to already know the IP address of a DNS server. For instance, a computer may be configured to always use
	1.0.0.1
	As the DNS server

In the olden days, IT admins needed to manually set an endpoint's DNS server
	Today we rely on auto-configuration services to do this automatically. --> [[DHCP]]

# ![[Recursive DNS Server]]
