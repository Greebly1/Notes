A #Legacy network protocol used to connect and control a computer over a network

earliest method for remote access
	Used for commands, access files, manage resources

Used extensively for
	Server administration, troubleshooting, and data retrieval

# Security Concerns
When telnet was first developed, it was during a time where the internet was still mostly just for universities.
Most telnet connections were made over a LAN

for this reason Telnet was not encrypted.
	Password, usernames, files, etc create security concerns

Replaced by [[SSH]] for these reasons

# How to use
First of all a telnet server needs to be running and listening on port 23

	telnet domainName
instead of a domain name, an IP address can be used
	Using a domain name also performs a [[DNS]] query on the backend