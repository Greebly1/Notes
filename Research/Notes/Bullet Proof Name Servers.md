When a domain is caught doing illegal activities such as selling black market goods and services, authorities can shut it down through several means
1. Raid the server and physically shut it down
		Server must be in their jurisdiction
		Does not work with proxy servers (since that isn't the main server)
		Does not work on Botnets that host the server (or host proxies pointing to it)
2. Order the name server to blacklist the domain

# Bullet Proof Servers
A bullet proof name server is an [[Authoritative Name Server]] that ignores orders from legal entities, and is often out of their jurisdiction

These bullet proof name servers usually get their IPs blocked
	So they used [[Proxy Server]]s to circumvent that.

# How they host IPs
So name servers don't *get given IPs*, 
	Malicious actors obtain these domains through several means
1. Using hosting providers in places with lax laws and oversight
2. Rent IP space from legitimate providers
3. Hijacking unused IPs (not caught very quickly), exploits [[BGP]]
4. Fake companies look legit

These actors then tell higher level name servers that their domain IP is stored in *this* server
	That is almost always a proxy server that points to their bulletproof name server

# [[Fast Flux]]
When discovered as malicious, high level name servers blacklist the proxies that point to the bulletproof name servers.
	A technique called fast flux is used to circumvent this